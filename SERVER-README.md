# Server Readme

This is a documentation of helpful information about the server usage.

## Open Ports

See <https://github.com/eclipse-thingweb/.github/blob/main/SERVER.md#ports-documentation>

## Web Server 

We use Apache 2

HTMLs are available at /var/www/html

## Screens

We use multiple screens to manage different services.
Please load services in dedicated screens after a restart of a service or of the server.

* List available screens: `screen -list`
* Create a new screen: `screen -dmS myScreen`
* Enter screen with ID: `screen -r <NUMBER>`
* Leave screen: `ctrl+a  d`
* Rename a screen: `ctr+a : sessionname <NAME>`

## Update node-wot

* walk into /home/vserver/thingweb.node-wot
* update repo: "git pull"
* build: "npm ci", "npm run build"

e.g., start TestThing again in a screen

`wot-servient testthing.js counter.js coffee-machine.js > ../logs/TestThing-004.log 2>&1`

OR

`node packages/cli/dist/cli.js examples/testthing/testthing.js examples/scripts/counter.js examples/scripts/smart-coffee-machine.js `

## Start wot-fxui (in background / server mode)

cd wot-fxui/
./gradlew -b jpro.gradle jproRestart
