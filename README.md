# Hubot-save-links

A hubot script that saves links
At the moment it supports local redis installations or redis togo service attached in Eroku

See [`src/save-links.js`](src/save-links.js) for full documentation.


## Installation

Install [Hubot](https://hubot.github.com/)

In hubot project repo, run:

`npm install hubot-save-links --save`

Then add **hubot-save-links** to your `external-scripts.json`:

```json
[
  "hubot-save-links"
]
```


## Sample Interaction

The script saves links from messages, discarding duplicates
If you want to try locally simply launch hubot
```
bin/hubot
```
```
hubot>> hubot  http://example.com
hubot>> hubot  hello, check this: http://anotherexample.com
```
The above links will be saved in redis


## Debug

If you want a verbose logging on the console simply launch hubot with the env variable 
DEBUG

```
DEBUG=save-links bin/hubot
```
more verbose:

```
DEBUG=* bin/hubot
```

## Test

Well, it's version 0.0.4, the fuctionaloty is small, will do for sue :P

## TODO

Check the [open issues](https://github.com/cirpo/hubot-save-links/issues)
