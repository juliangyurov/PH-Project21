## [Project 21: Local Notifications](https://www.hackingwithswift.com/read/21/overview)
Written by [Paul Hudson](https://www.hackingwithswift.com/about)  ![twitter16](https://github.com/juliangyurov/PH-Project6a/assets/13259596/445c8ea0-65c4-4dba-8e1f-3f2750f0ef51)
  [@twostraws](https://twitter.com/twostraws)

**Description:** Send reminders, prompts and alerts even when your app isn't running.

- Setting up

- Scheduling notifications: `UNUserNotificationCenter` and `UNNotificationRequest`

- Acting on responses

- Wrap up

  
## [Review what you learned](https://www.hackingwithswift.com/review/hws/project-21-local-notifications)

**Challenge**

1. Update the code in `didReceive` so that it shows different instances of `UIAlertController` depending on which action identifier was passed in.

2. For a harder challenge, add a second `UNNotificationAction` to the alarm category of Project21. Give it the title “Remind me later”, and make it call `scheduleLocal()` so that the same alert is shown in 24 hours. (For the purpose of these challenges, a time interval notification with 86400 seconds is good enough – that’s roughly how many seconds there are in a day, excluding summer time changes and leap seconds.)

3. And for an even harder challenge, update Project2 so that it reminds players to come back and play every day. This means scheduling a week of notifications ahead of time, each of which launch the app. When the app is finally launched, make sure you call `removeAllPendingNotificationRequests()` to clear any un-shown alerts, then make new alerts for future days.
