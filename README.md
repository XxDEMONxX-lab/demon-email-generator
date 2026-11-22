# Demon Mail

A responsive disposable email website powered by the public [mail.tm](https://mail.tm/) API.

## Features
- Create a real temporary mailbox on an available mail.tm domain.
- Receive and refresh incoming messages automatically every 12 seconds.
- Read message sender, recipient, subject, date, and text content.
- Copy the generated address and delete the mailbox.
- Responsive dark UI; no build step or framework required.

## Run
Open `index.html` in a modern browser, or serve this directory with any static HTTP server:

```sh
python3 -m http.server 8080
```

Then visit http://localhost:8080.

## Notes
- This is a disposable inbox, not a sender or a permanent email provider.
- Mailbox creation and message delivery depend on mail.tm availability, its domain policy, and API limits.
- The browser communicates directly with mail.tm. No application server or database is required.
- The account password and API token exist only in page memory. Refreshing the page loses access to the current mailbox.
- Do not use temporary addresses for sensitive accounts, password recovery, or important correspondence.
