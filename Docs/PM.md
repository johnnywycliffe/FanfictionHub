# PM system design

PMs are used to allow two users to communicate. However, there's several systems in place to make the place more friendly.

There is a sender and a receiver.

## Systems

- Generic
  - White/Blacklist: Users can add other users to a private blacklist
  - PMs can be turned on and off completely for a user
  - Word blacklist: Disallow messages with certain words in them
  - Sanitization: Automatically remove code, etc.
  - Toggle for automatically blocking links
- Sender
  - Spell check
  - Before the message is sent, show a preview of the message
- Receiver
  - Notifications of new message
  - Option to reply
  - Option to block/report user

