Nice Things
===========

A Crontab exercise<br>
By: Christopher Fryman

[Learn more about crontab] (https://en.wikipedia.org/wiki/Cron)

a fun little app that says nice things to you.
To encourage you on a regilar basis, do these things.

1) save the file on your system<br>
`sudo curl https://raw.github.com/farfromguam/nice-things/master/nice_things.rb > /usr/local/bin/nice_things.rb`

2) change the mode of the file to executable<br>
`chmod +x /usr/local/bin/nice_things.rb`

3) Edit your local crontab with the comand<br>
`sudo crontab -e`

4) Add one of these crontab entries

Execute Every 5 minutes:<br>
`*/5 * * * * /usr/local/bin/nice_things.rb`

Execute Every Hour:<br>
`0 */1 * * * /usr/local/bin/nice_things.rb`

Execute Monday Mornings at 9:05<br>
`5 9 * * 1 /usr/local/bin/nice_things.rb`

Every 10 minutes all day on your birthday<br>
`*/10 * D M * /usr/local/bin/nice_things.rb`

7) Check that your crontab has been saved
`sudo crontab -l`

6) If you find yourself not wanting encouragement<br>
run `sudo crontab -e` and remove your event
