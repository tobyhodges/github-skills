# Managing Notifications

## Specify the email address for each organisation

1. Click on your profile picture at the top-left of the GitHub window.
2. Choose _Settings_
3. Click _Emails_ and make sure your contact details are up-to-date
  4. e.g. if you have work and "hobby" projects on GitHub,
     you may want to include a personal email address as the primary
     and a work email address as a secondary
4. If you have more than one email address associated with your account,
   click on _Notifications_.
5. Scroll down to _Custom routing_.
   Here, you can specify at which email address you would like to receive
   notifications from repositories in each of the organisations you are
   a member of.
  6. I use a personal address for "hobby" projects and my work email for
     Carpentries-related repositories.

Any repositories that do not belong to an organisation i.e. those that exist
under your own account namespace (`github.com/tobyhodges/` for me) will
send their notifications to the primary email associated with your account.

## Adjust your notification level for a repository

Navigate to a GitHub repository e.g. [tobyhodges/github-skills](https://github.com/tobyhodges/github-skills)
and click on the _Watch_ button
(this might say _Unwatch_, if you chose a repository that you are already subscribed to)
, near the top-left of the window, with an :eye: icon.
Choose your preferred level of notifications for that repository.
Use _Custom_ if you want to receive only particular types of notification.
Choosing _Ignore_ will mean that you will not be notified about anything on
this repository,
_even if you are mentioned, or if there is activity on an issue/pull request that you have participated in_.

## Filtering and organising email notifications

If you are subscribed to anything more than a few repositories on GitHub,
you are likely to receive _a lot_ of notification email.
It is possible to turn off all email notifications
(go to the _Settings_ -> _Notifications_ page as described above)
and rely on your notifcations page at https://github.com/notifications .
I tried this for a while and found that I very quickly lost track of what was
going on and what I needed to be paying attention to.

So, assuming you want to keep receiving notifications by email,
how can you handle that deluge of notifications in a way that enables you to
distinguish between the things that need your attention right away
and the things it is okay to come back to later/hit "mark as read"
because you _just can't right now_?

Here is how to send all GitHub notifications to their own folder in Apple Mail:

1. Click on the _Mailbox_ dropdown menu,
   and choose _New Mailbox..._
   A new window should pop up, inviting you to configure the new mailbox.
2. Make sure the _Location_ field is pointing to the account where you receive your
   GitHub notifications. (If you receive notifications in multiple accounts,
   you will need to follow these steps multiple times.)
   Now give your new mailbox a name, e.g. _GitHub Notifications_.
1. Click on the _Mail_ dropdown menu, and choose _Preferences_.
2. Navigate to the _Rules_ tab, and click _Add Rule_.
3. Using the dropdowns and the text fields, create a rule that redirects any
   message from `notifications@github.com` to your new mailbox.
   ```
   If all of the following conditions are met:
   From is equal to notifications@github.com

   Perform the following actions:
   Move message to mailbox: GitHub Notifications
   ```

GitHub provides a way to differentiate between different kinds of notification,
based on the email addresses it includes in the CC field of the message.
We can use this to highlight particular messages based on the type of notification
you are receiving.
For example, here is how to tell Apple Mail to highlight any notifcation telling
you that your GitHub handle was mentioned:

1. Click on the _Mail_ dropdown menu, and choose _Preferences_.
2. Navigate to the _Rules_ tab, and click _Add Rule_.
3. Using the dropdowns and the text fields, create a rule that flags any
   message that includes the `mention@noreply.github.com` address in CC.
   ```
   If all of the following conditions are met:
   CC contains mention@noreply.github.com

   Perform the following actions:
   Mark as flagged: Yellow
   ```

You can also add additional rules to make these filtering steps more advanced.
(Click the `+` symbol while setting up your filter, to add new rules.)
But watch out! I have found that it is easy to create conflicting/overlapping
rules that can result in confusing behaviour and missed notifications.
My advice is to keep it simple and then watch out for those flagged messages
that are likely to be most important to you.

Finally, the above is specific to one mail client - Apple Mail.
Other mail programs are likely to have similar functionality,
and many have more advanced features and better filtering,
e.g. that will help you to avoid the conflicts between rules that I mentioned before.
