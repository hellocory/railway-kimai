# Kimai - Timetracking for Businesses and Freelancers
[Kimai](https://www.kimai.org/) is an Open Source time tracking application. This one-click-deployment will be all you need to use for Railway to set it up.

# One-click-setup
Click below to deploy to railway.

[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/E3MdZb?referralCode=QkFCyI)

# Railway Deployment Instructions
1. Add your admin email & password.
2. Remove the admin email & password environment variables after build (they're no longer needed).

# Troubleshoot:
TLDR: This is my first template with Railway so there may be more improvements to be made. Let me know if there is more that I can do to improve on this template if needed! I can add addon's later as well.
<table>
<tr>
<th>ISSUE</th>
<th>SOLUTION</th>
</tr>
</tr>
<tr>
<td>
The app doesn't load
</td>
</td>
<td>
Make sure to REMOVE the URL that is assigned to your "Kimai" application, and reassign a newly generated domain or a custom one with the port of `8001`.
</td>
</tr>
<tr>
<td>
Invalid credentials
</td>
</td>
<td>
You must make sure the MYSQL_URL has `?charset=utf8mb4&serverVersion=8.3.0` appended to end of the URL. I'm not sure if I can get it to work by default with the template.
</td>
</tr>
<tr>
<td>
Emails don't work
</td>
</td>
<td>
Refer to https://www.kimai.org/documentation/emails.html to see how the `MAILER_URL` & `MAIL_FROM` environment variables work.
</td>
</tr>
</table>

