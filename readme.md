Nice Things
A Crontab exercise
By: Christopher Fryman

[Learn more about crontab] (https://en.wikipedia.org/wiki/Cron)

a fun little app that says nice things to you.
To encourage you on a regilar basis, do these things.

1) save the file on your system
usr/local/bin

2) Edit your local crontab with the comand
"crontab -e"

3) Add one of these crontab entries

Execute Every 5 minutes:
*/5 * * * * /usr/local/bin/nice_things.rb

Execute Every Hour:
0 */1 * * * /usr/local/bin/nice_things.rb

Execute Monday Mornings at8:05
5 9 * * 1 /usr/local/bin/nice_things.rb

Every 10 minutes all day on your birthday
*/10 * D M * /usr/local/bin/nice_things.rb

If you find yourself not wanting encouragement
open "crontab -e" and remove your event