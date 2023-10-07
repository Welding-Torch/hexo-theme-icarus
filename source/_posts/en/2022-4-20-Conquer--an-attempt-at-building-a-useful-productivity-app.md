---
layout: post
title: Conquer - an attempt at building a useful productivity app
date: 2022-4-20
toc: true
---

_This blog is going to be about a productivity app - its journey, obstacles, technical and product details._

the app is called Conquer ([web](https://conquer-goals.netlify.app), [android](https://github.com/devout-coder/conquer-rn-app/releases))

<!-- more -->

## Contents

- How Conquer came into being
- How it works
- Technical details

Its gonna be a long one, get some popcorn and hang tight!

## How Conquer came into being

It was November 2020, and I was having the time of my life writing automation scripts and a personal website. JEE was a few months away, most of my friends who were JEE aspirants had finished their portions and I realised that I gotta start the portion. But there was a hiccup - I wasn’t able to find a decent tool, with the features, the UI/UX I personally wanted to plan my sprint. So instead of starting with PCM my caveman brain decided to start building. I had used React for a basic CRUD app. So I decided to use it for Conquer as well and till Jan I was able to hack together the tool which I had visualized.

I still used to waste a lot of time and I wondered what if Conquer reminds me that I gotta study when I waste time scrolling on Twitter or Insta? I really believed that this is a very cool idea, so I decided to build this no matter what it takes and started learning React Native.

After CET, I began working on Conquer’s android app. But when I built all the features which the web app had and began working on Nudger(part of my app which would nudge me on wasting time) I realised that there is no library built in React Native which can help me track apps and I would have to learn native android development using Java. I got into native development, learnt it enough to resume working on Nudger. I still wasn’t able to understand how to track which app is running in the background. I was really gonna give up on it, but then one night I had my eureka moment when I was wondering how the app blockers work. I dug into it, found that they use something called “accessibility service”. It took me a lot of nights and sweat but finally I did pull the app off till Nudger.

I participated in a hackathon around the same time and I realised how cool it would have been if I could share the common tasks with my teammates on Conquer. So I built that feature into the android app.

## How it works

Conquer allows users to divide their tasks and goals into five segments: daily, weekly, monthly, yearly and long term. Create and prioritse tasks in all these sections.

![Daily Todos Page](/gallery/conquer-images/daily-todos-page.png "Daily Todos Page")

![Weekly Todos Page](/gallery/conquer-images/weekly-todos-page.png "Weekly Todos Page")

![Monthly Todos Page](/gallery/conquer-images/monthly-todos-page.png "Monthly Todos Page")

![Yearly Todos Page](/gallery/conquer-images/yearly-todos-page.png "Yearly Todos Page")

![Long Term Todos Page](/gallery/conquer-images/long-term-todos-page.png "Long Term Todos Page")

![Creating a task](/gallery/conquer-images/creating-a-task.jpg "Creating a task")

Had planned to get done with something this week but couldn’t? Conquer lets you postpone tasks in all sections and lets you know how many times you have postponed something. Wanna get a group project done and make sure your teammates are updated with unfinished tasks? With Conquer you can add friends and share tasks with them. This is where the similarities of web and android app end.

![Sharing Tasks](/gallery/conquer-images/interface-for-sharing-tasks.png "Sharing tasks")

Nudger is the feature which lets you blacklist apps and websites and notifies you about unfinished tasks, nudges you in Ashneer Grover’s iconic dialog “Bhai kya kar raha hay tu mazak hay kya” and navigates back to your home screen.

![Nudger](/gallery/conquer-images/nudger.jpg "Nudger")

![Nudger Alerts](/gallery/conquer-images/nudger-alerts.jpg "Nudger Alerts")

## Technical details

As I said before, I have used React to build the web app and Firebase’s services for authentication and database. The web app is hosted on Netlify. The android app is primarily built using React Native. The code which detects which app is running in background and alerts user is written in Java(unfortunately). What the java code does is, triggers an [accessibility service](https://developer.android.com/guide/topics/ui/accessibility/service) whenever window changes, checks if the new app is blacklisted and starts an alarm using [Alarm Manager](https://developer.android.com/reference/android/app/AlarmManager) if it is, then pushes a notification and takes user home when the alarm goes off.

Thats all for today, hopefully I haven't bored you, thank you for patiently sticking with me. If you have any questions, thoughts etc. feel free to hit me up on any of my socials ([Twitter](https://twitter.com/devout_coder), [Insta](https://instagram.com/devout_coder), [Email](mailto:awessssomepro@gmail.com)).

Feel free to reach out to any of us geeks on our [WhatsApp Group](https://chat.whatsapp.com/K3NrW5tPwrsHhfbdYstjLl)
