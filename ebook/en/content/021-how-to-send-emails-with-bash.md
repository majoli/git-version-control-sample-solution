# Sending emails with Bash and SSMTP

SSMTP is a tool that delivers emails from a computer or a server to a configured mail host. 

SSMTP is not an email server itself and does not receive emails or manage a queue. 

One of its primary uses is for forwarding automated email (like system alerts) off your machine and to an external email address.

## Prerequisites

You would need the following things in order to be able to complete this tutorial successfully:

* Access to an Ubuntu 18.04 server as a non-root user with sudo privileges and an active firewall installed on your server. To set these up, please refer to our [Initial Server Setup Guide for Ubuntu 18.04](https://www.digitalocean.com/community/tutorials/initial-server-setup-with-ubuntu-18-04)

* An SMTP server along with SMTP username and password, this would also work with Gmail's SMTP server, or you could set up your own SMTP server by following the steps from this tutorial on [How to Install and Configure Postfix as a Send-Only SMTP Server on Ubuntu 16.04](https://www.digitalocean.com/community/tutorials/how-to-install-and-configure-postfix-as-a-send-only-smtp-server-on-ubuntu-16-04)