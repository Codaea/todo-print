# Todo Printer

A simple webapp using alpine.js for printing todo tasks via a thermal printer

## Features
- Print tasks and subtasks
- Easy printer setup
- Keyboard shortcuts for quick printing

## Setup/Usage
To use with your own printer, setup [Simpleprint](https://github.com/codaea/simpleprint) and set the printer IP and port in the input field provided in the app. (make sure you have your `http://` prefix!)

I just use internal IP addresses across my tailnet, but whatever floats your boat (Maybe don't expose it over the internet though, thats a bad idea.)

You can also just host the index.html through whatever your favorite platform is, you don't have to use my domain/webserver.


## Troubleshooting

Why is it not printing?

I'd start by checking developer console for any errors

### Mixed Content

Chrome by default blocks mixed content (HTTP content on HTTPS sites). If you see errors about mixed content, so if you are using a http url for your printer, you can either:
- use a https url via a reverse proxy
- disable mixed content in site settings (check out [this guide](https://stackoverflow.com/questions/18321032/how-to-get-chrome-to-allow-mixed-content))

