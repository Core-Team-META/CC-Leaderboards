# Leaderboards - README
1.0.2 - 2021/02/01
by [Nicholas Foreman](https://www.coregames.com/user/f9df3457225741c89209f6d484d0eba8)

Leaderboards is a component that simplifies the process of adding a global leaderboard to a game. It is as simple as dragging
and dropping a leaderboard template into the hierarchy and adjusting to meet your needs.

1. Creating a Global Leaderboard
    - Go to the "Global Leaderboards" tab in the editor: View > Global Leaderboards
    - Click "Create New Leaderboard"
    - Follow the prompt to create your leaderboard

2. Setup
    - Drag and drop "Leaderboard Dependencies" into the hierarchy
    - Note: Make sure this is the only version in the hierarchy
    - Drag and drop either a "World Leaderboard" or "Interface Leaderboard" into the hierarchy
    - With the Global Leaderboards view still open, select the World/Interface Leaderboard object and locate the LeaderboardReference custom property. It should say *Missing Reference*. Drag your leaderboard from the Global Leaderboards view onto the Properties view to assign the custom property.
    - Alter custom properties for each template as needed.

3. Usage

    The most basic usage includes KDR, Kills, and Deaths by dragging the template (world or interface) into the hierarchy and
adjusting LeaderboardStat to be KDR, KILLS, or DEATHS. However, more advanced usage includes Resources in which you can
set LeaderboardStat to be RESOURCE and change ResourceName to any resource of your choosing, such as "Money".

4. Leaderboard Dependencies

    "Leaderboard Dependencies" is a single template that must be in the hierarchy and remain in the hierarchy. There should 
only be one of this template in the hierarchy. It handles the persistent tracking of resources, kills, deaths, and kdr.
Having multiple of this in the hierarchy can cause unwanted bugs and possible corruption. Not including it in the hierarchy
will make each of the leaderboard template not function, either.

5. World Leaderboard

    A "World Leaderboard" is a physical panel in the world utilizing WorldText to display rankings.

6. Interface Leaderboard

    An "Interface Leaderboard" is a UI panel utilizing UI elements to display rankings on the player's screen. With slightly 
more customization, included is the ability to toggle and ease in/out the UI.

7. Monthly, Weekly or Daily Time Frames

    - Leaderboards that show Monthly, Weekly and Daily scores can be created with a single entry in the Global Leaderboards menu.
    - For each desired time frame, add a copy of the World/Interface templates, and assign the same leaderboard entry to each one.
    - Then, for each template, configure the "LeaderboardType" custom property to say GLOBAL, MONTHLY, WEEKLY or DAILY.

8. Discord

    If you have any questions, feel free to join the Core Hub Discord server: discord.gg/core-creators
We are a friendly group of creators and players in the Core community. Everyone is welcome to play games together or learn about game dev!
