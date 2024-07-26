# NGINX Server Profiler:

Track the user activity & errors logs on [Nginx](https://nginx.org/en/) using [Cron](https://crontab.guru/) & [Docker Compose](https://docs.docker.com/compose/). It sends the user logs as a user session when a user requests the Nginx server this will help to demonstrate managing authentication, initiating and concluding activities, and overseeing state transitions.
This will send user logs through Sendmail, a lightweight command line [SMTP](https://github.com/zehm/sendEmail) email client every minute by using a cron job. To provide flexibility & security I have used a Docker container to separate any process into its own Docker container, or one service per container.
