# homeassistant
My Smart Home

## Mising files
Some files are missing in this repo due security or privacy reasons, these files are needed to run this configuration:
- google_calendars.yaml
- .google.token
- zones.yaml
- secrets.yaml

## Used services / modules
My smart home is heavily based on Ikea's Tradfri devices but I'm also using some other external stuff:
- Google Calendar
- Google Chromecast
- Sun
- DarkSky
- Life360
- MessageBird
- Flux

## Automations
### Melding - Bak buitenzetten
I'll get a notification using MessageBird when I have to put the garbage bin outside.
### Melding - Later thuis
SO get's a notification when I'm late from work when she is also home.
### Iedereen Weg - Lichten Uit
When nobody is home turn out all lights in the livingroom.
### Buitenverlichting aan bij zonsondergang
When it's getting dark outside turn some light's in the garden on.
### Buitenverlichting uit om 1 uur
Turn off the light's in the garden at 1 AM.
### Zet automations voor de dag aan
New day! Activate all relevant automations for this day.
### Start Film / Start Serie
When starting a movie or tvshow on the Chromecast, turn down / off the lights.
### Pauze Chromecast
When pauzing or stopping the Chromecast that's playing a movie or tvshow turn on the lights again.
### Schakel keuken werklicht in / Schakel keuken werklicht uit
Turn on the extra kitchen counter lights when motion is detected and other lights in the kitchen are already on.
### Goedemorgen werkdag
Turn on the livingroom lights ONCE when motion is detected in the hallway between 7 AM and 12 PM and it's dark enough.
### Lichten aan bij zonsondergang
Turn on the livingroom lights when it's getting dark outside and the Chromecast is not playing something relavant.
### Lichten uit bij zonsopgang
Turn off livingroom lights when it's light enough outside.
### Voordeur hoog
Set the light at the frontdoor high when someone arrives at home. This will be automatically turn down again by: Voordeur Auto Laag
### Voordeur Auto Laag
Turn down the lights at the frontdoor after 10 minutes when they were set to high.
## Thuis Komen
Reanimate the home (aka start homecoming script) when someone comes home.
## Cancel Homecoming AutoOff
Cancel the automatic shutdown when motion is detected in the hallway (this is a solution to false positives).
## Buitenverlichting laag
When the livingroom light's are turned off set gardenlight's low.

## Scripts
### Welkom thuis
Turns the light's in the hallway and livingroom on, wait 20 minutes and turn them off again. This script will be cancelled when there is motion detected in the hallway.

## Sensors
### PiHole
Shows the number of blocked requests
### History sensors
Shows percentage of time (per week) someone is:
- At work
- At home

Also displays how many hours the light's are turned on in the livingroom (weekly).
### dusk
Returns yes when it's outside dark enough to put some light's on inside.
### chromecast_movie
Return yes when the Chromecast is playing a movie.
### chromecast_tvshow
Return yes when the Chromecast is playing a tv show.