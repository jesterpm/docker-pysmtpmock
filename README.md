Mock SMTP Server which displays the received messages on stdout.

The server is the python smtpd module in debug mode. The default command is:

    python -m smtpd -n -c DebuggingServer localhost:25

The received message looks something like:

    ---------- MESSAGE FOLLOWS ----------
    from: test@example.com
    to: test2@example.com
    subject: Hello

    Hello World
    ------------ END MESSAGE ------------
