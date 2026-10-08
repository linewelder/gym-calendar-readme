# Gym Calendar

_Note: The source code is private for the time being. This repo is a temporary stand-in for the app web page during development._

<div align="center">
<img src="icon.png" width="128" alt="Gym Calendar logo">
</div>

Plan your workouts and track your progress, offline or online. A tool rather than a service: cloud features are optional and nothing shows up in your face that you didn't ask for.

<div align="center">
<img src="https://github.com/linewelder/gym-calendar-readme/blob/main/screenshots/demo.gif?raw=true" width="400" alt="App demo">
<p><i>Note: The demo has a reduced framerate to save on the file size</i></p>
</div>

## Features

### Plan today's workout

Set the goals for today's workout.

![Workout planning screen](screenshots/workout-overview.png)

### Record your sets

Use the set-rest timer, or enter results directly using an effortless UI.

![Set-rest timer](screenshots/timer.png)

## In development

- Multi-week plans with [periodization](https://en.wikipedia.org/wiki/Sports_periodization)
- Progress history
- Cloud sync and plan sharing (Ktor backend)

## Architecture

- **Native Android app:** Kotlin, Jetpack Compose, Hilt, Room
- **Offline-first:** all data lives on the device and the app is fully usable without a connection, since gyms often have poor reception. Cloud sync is designed in from the start.
