# Kyujin Bot: screenshots for Discord's privileged intent review

Kyujin Bot (application ID 1532200649930833920) is a private bot that runs
only in kpopfriends (KPF) and its owner's private server.
Privacy policy: https://gist.github.com/greatgreatasset/50a503f2edc75b1e12e856678e239d77

## Message Content intent

### 1. Archive viewer: a deleted message kept in the moderation log
The read-only viewer on the owner's PC (localhost). The message was deleted
on Discord; the archive keeps it with a "deleted" marker so a reported post
can still be reviewed.

![Deleted message in the archive viewer](01-archive-viewer-deleted.png)

### 2. Archive viewer: edit history of a message
Every edit is kept, so what a post said when it was reported can be checked.

![Edit history in the archive viewer](02-archive-viewer-edit-history.png)

### 3. Delete alert DM (owner's private server)
When a message is deleted on the private server, the bot DMs the owner the
archived text. This needs the message content.

![Delete alert DM](03-delete-alert-dm.png)

### 4. Honeypot: anti-spam
The hidden honeypot channel's status message (banned compromised accounts
so far) and a catch announcement. The archive is used to clean up the spam.

![Honeypot status and announcement](04-honeypot.png)

### 5. Media relay: the #kpopfriends post
A member's post in KPF's #kpopfriends tagging an idol ping role.

![Post in #kpopfriends](05-relay-kpf-post.png)

### 6. Media relay: the copy in the private server, with review buttons
The same post relayed by webhook to the matching channel in the owner's
private server, with the Approve / Delete / Always approve / Ignore buttons.
Copying it needs the post's links (content) and attachments.

![Relayed copy with review buttons](06-relay-copy-with-buttons.png)

### 7. Link card for an X/Twitter link posted in chat
The bot has to see the link in the message to reply with the post's text,
media and counts.

![Link card](07-link-card.png)

## Server Members intent

### 8. The rank role ladder
Server Settings → Roles: the 12 stacking rank roles, with the base role
(LewdNewb) that every member is meant to hold from the moment they join.

![Rank roles](08-rank-roles.png)

### 9. Audit log: Kyujin Bot gives the base role
"Kyujin Bot added the role LewdNewb" with reason "New member". Today this
can only happen when the member first posts; with the Server Members intent
it happens on join.

![Audit log entry](09-audit-log-newb.png)

### 10. /rank reply
The rank commands assume every member holds the base rank role.

![/rank reply](10-rank-reply.png)

## Other

### 11. /role panel in #ping-roles
The slash-first design: the bot's commands are slash commands.

![Role panel](11-role-panel.png)

### 12. Developer Portal: Public Bot off, privacy policy linked
![Portal settings](12-portal-settings.png)
