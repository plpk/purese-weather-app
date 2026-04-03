# Purese: AI-Powered Minimalist Weather App

[![App Store](https://img.shields.io/badge/App_Store-Published-blue?logo=apple&logoColor=white)](https://apps.apple.com/us/app/purese/id6744907444)
[![Platform](https://img.shields.io/badge/Platform-iOS_|_iPadOS_|_macOS-lightgrey?logo=apple)](https://apps.apple.com/us/app/purese/id6744907444)
[![Privacy](https://img.shields.io/badge/Privacy-Zero_Data_Collected-green)](https://apps.apple.com/us/app/purese/id6744907444)

Purese is a minimalist weather app that delivers AI-powered forecasts in a clean, simple interface while collecting absolutely no personal data. Published on the Apple App Store.

**[Download on the App Store](https://apps.apple.com/us/app/purese/id6744907444)**

## Features

- **AI Weather Reports** · Natural-language weather summaries powered by Google's Gemini API, tailored for kids, adults, and older adults
- **Next-Day Forecast** · Extended AI-generated forecast with suggestions for planning ahead
- **Current Conditions** · Temperature, "feels like," humidity, and wind speed at a glance
- **City Search & Auto-Location** · Search by city name or detect weather for your current location
- **Privacy-First** · Zero personal data collected. No tracking. No ads.
- **iOS-Native Design** · Clean, refreshed interface inspired by Apple's design language

## Tech Stack

| Component | Technology |
|-----------|-----------|
| Framework | Flutter (Dart) |
| AI Integration | Google Gemini API |
| Weather Data | OpenWeatherMap API |
| Location | Geolocator package |
| Networking | HTTP package |
| Platforms | iOS, iPadOS, macOS (Apple Silicon) |

## Architecture

Purese integrates two external APIs into a unified experience. OpenWeatherMap provides raw weather data (temperature, humidity, wind, conditions), which is then passed to Google's Gemini API to generate natural-language weather reports with context-aware suggestions. The Gemini integration produces different report variants based on audience (children, adults, seniors), making weather information accessible across age groups.

The app uses Flutter's cross-platform framework with platform-specific configurations for iOS and macOS. Location services are handled through the Geolocator package with graceful fallback to manual city search.

## Development Approach

Purese was developed using AI-assisted development with AI coding assistants (Claude, ChatGPT) writing the Flutter code while I directed the process: defining the product requirements, selecting the tools and APIs, making architecture decisions, debugging and iterating, and navigating Apple's full App Store submission and review process independently. The achievement here is product shipping, API integration, and product thinking. AI-assisted development is a real and emerging skill category, and this app is a working example of it.

## About This Repository

This repository contains the development codebase for Purese. The published App Store version (v2.0.2) includes additional features, design refinements, and the "Purese" branding that evolved beyond what is reflected in this codebase.

## Local Development

```bash
# Clone the repository
git clone https://github.com/plpk/purese-weather-app.git

# Install dependencies
flutter pub get

# Create a .env file with your API key
echo "OPENWEATHER_API_KEY=your_key_here" > .env

# Run the app
flutter run
```

## Privacy Policy

Purese does not collect, store, or transmit any personal data. The app requests location access solely to provide weather for your current position. This data is sent directly to the weather API and is never stored or logged. [Full privacy policy](https://github.com/plpk/purese-weather-app/blob/main/privacypolicy)

## Author

**Louis Kunasek** · [GitHub](https://github.com/plpk) · [LinkedIn](https://www.linkedin.com/in/LouisKunasek) · Louis.Kunasek@outlook.com
