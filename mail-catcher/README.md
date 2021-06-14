# Mail Catcher

Using MailHog and Caddy, this snippet allows you to setup a catch-all mailbox - useful for testing email delivery and formatting from your application.

Caddy is used to provide basic authentication, so not just anyone on the Internet can access your test messages. 
See the Caddyfile for more information on authentication.

The web interface is configured on port 8025 and the SMTP protocol is exposed on localhost (127.0.0.1) on port `1025`.

Example `.env` file:
```
MAIL_DRIVER=SMTP
MAIL_HOST=127.0.0.1
MAIL_PORT=1025
MAIL_USERNAME=
MAIL_PASSWORD=
```