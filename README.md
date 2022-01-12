
# Time tracker for support and tickets

This project exposes a single page, for clients that subscribes for support.

We use milestones and issues in gitlab to track our work, then our client can have a picture of its support consumption.

## How to use it

In gitlab, create a "support" project for the client. In this project, create a new access token with only "read api" role.

Send to the client its own timetracking url : 

https://timetracker.please-open.it?token=ACCESS_TOKEN

Create a milestone per support billing.

In this milestone, start with an issue which is the credit. use "/estimate" tag with the amount sold to the client.

For each support, create an issue (with all details) and "/spend" with the time spent on the issue.

It supports Markdown in milestones and issues.

## Tech

uses : 

- [mustache.js](https://github.com/janl/mustache.js/)
- [mustache-wax](https://github.com/jvitela/mustache-wax)
- [bootstrap](https://getbootstrap.com)
- [showdown](https://github.com/showdownjs/showdown)