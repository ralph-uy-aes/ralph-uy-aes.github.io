---
title: "E59: Learn to deploy a Nextjs app"
published: true
morea_id: experience-test-deployment-vercel
morea_type: experience
morea_summary: "Deploy nextjs-application-template-react to Vercel"
morea_sort_order: 3
morea_start_date: "2025-04-04T23:00:00"
morea_labels:
---

# E59: Deploy nextjs-application-template

For this experience, you will learn how to deploy the nextjs-application-template app to Vercel in order to make it available for anyone to use who has access to the Internet and a browser.  You will also learn how to monitor your "production" database at Vercel, and how to set up application performance monitoring.

To do this, perform all the steps in the following readings in order:

  1. [How to deploy a Nextjs application to Vercel](./reading-vercel.html).
  2. [How to inspect your Supabase database on Vercel using pgAdmin](https://supabase.com/docs/guides/database/pgadmin)

# Linking Supabase to pgAdmin
In order to find the hostname, port, username, and password, go to your Vercel Supabase dashboard in the tab **Storage**. Click on **Show secret** and you will only really need the first URL called `POSTGRES_URL`.

{% include medium-img.html url="dashboard-supabase.png" %}

The text highlighted in red is your Username. 
The text highlighted in blue is your Password (obfuscated here).
The text highlighted in yellow is your Host name/ address.
The text highlighted in green is your Port.

If you are getting errors, that you don't understand how to resolve, feel free to ask a #smart-question.

### Submission

By the date and time indicated on the Calendar page, please finish all of these steps. Create two screenshots:

  1. Your Nextjs application (retrieved using a URL like "https://my-nextjs-application-rho.vercel.app/").
  2. Your pgAdmin screen showing a connection to your Nextjs application.

Post them to the #deployment channel.
