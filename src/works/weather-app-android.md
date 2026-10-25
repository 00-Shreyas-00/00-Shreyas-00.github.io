---
title: Weather App for Android
order: 3
featured: false
year: 2026
category: Android
stack: Kotlin, Jetpack Compose, MVVM, Coroutines, Retrofit
thumbLabel: Kotlin · Jetpack Compose
summary: An Android weather application built with Kotlin, Jetpack Compose (Material 3), MVVM architecture, Coroutines, and Retrofit with OkHttp, using the OpenWeatherMap API.
repo: https://github.com/00-Shreyas-00/Weather-app-Android
---

## Features

### Search, refresh and error handling

The app loads Pune by default and lets you search for any city, with validation for empty input. It shows the current condition, temperature, feels-like temperature, daily high and low, humidity, wind speed and pressure. When a search fails or the network drops, a dismissable error banner appears while the last valid weather stays on screen.

## Architecture

### MVVM with Compose

The UI is built with Jetpack Compose (Material 3) and follows MVVM, with Kotlin Coroutines and StateFlow for asynchronous work. Networking uses Retrofit and OkHttp with a logging interceptor, Gson for JSON parsing and Coil for weather icons. The app targets Android 14 (API 34) with a minimum of Android 8.0 (API 26).
