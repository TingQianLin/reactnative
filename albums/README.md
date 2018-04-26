# Album List App

An App to list the albums.\
Uses a very simple Go server to serve the json data for demo.

## Initial Steps

1. Install [Go](https://golang.org) if you don't have one.
2. `cd` to working directory and run `go run main.go` to serve the demo data for the app.
3. Open your AVD.
4. Run `adb reverse tcp:8080 tcp:8080` to mapping localhost port to AVD port.
5. Run `react-native run-android` to run the app.

### Clear Cache

1. `cd` to `./android` directoy.
2. Run `./gradlew clean`.