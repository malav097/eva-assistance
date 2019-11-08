# eva-assistance

A personal telegram bot assistance written in python3.

This is a telegram bot that i created and now i use in a daily basis. I hosted it in 
a AWS EC2 Instance and it communicates with google calendar API, Wikipedia API, Accuwather
API and of course, Telegram API.

The bot is installed as a `systemd service` and has the following features and functionalities.

### Execute commands

Execute commands inside the server that the bot is hosted in. You provide the telegram userid capable of running commands
in the configuration file. If someone else try to execute commands and is not authorized by you,
the bot will deliver a warning message to you.

By a security measure it is recommended that the system user who execute the bot process doesn't have sudo privileges.


### Daily messages

Daily messages that contains weather, to-do list and Google calendar Events.

### Weather query

1 day forecast or 5 day forecast weather query using the words `clima` or `clima completo`.

### Editable lists

todo.txt and notes.txt editable lists


### Google calendar events

Add and query google calendar events

![Screenshot_2019-11-07-17-33-18-898_org telegram messenger](https://user-images.githubusercontent.com/44653624/68440756-c76b7d80-01aa-11ea-877c-c4bb969503a5.png | width=100)

### Query anything 

Query anything and it will use regular expressions to try to find something useful in Wikipedia



# Bot commands:

`/execute` - Execute commands inside the server that the bot is hosted in.

`/todo` - Add a to-do element to the to-do list.

`/deletetodo` - Remove a to-do element from the to-do list.

`/noteadd` - Add an element to the note list.

`/deletetodo` - Remove an element from the note list.

`/eventadd` - Add event to google calendar with the following format `2019-12-27 Meeting with parthner`.
