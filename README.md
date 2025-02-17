
# MMM-Moon
Display a picture of the current moon phase along with moonrise and moonset times on your MagicMirror!

## How it works

Add the module to your MagicMirror like any other module, then add the "lat", "lon", and "timezone" parameters to your configuration file! The app calls the AstronomyAPI and gets an image with your parameters, then throws it onto your mirror!

## Screenshots
![Sample Picture One](./imgs/moon_pic1.png)

## Preconditions

* MagicMirror2 instance
* Node.js version >= 19
* npm


## Installation

Just clone the module into your MagicMirror’s modules folder and execute `npm install` in the module’s directory:

```bash
git clone https://github.com/EnderFlop/MMM-Moon
cd MMM-Moon
npm install
```

## Updating

Updating is as easy as navigating to the module’s folder, pull the latest version from GitHub and install.

```bash
git pull
npm install
```


## Configuration

| Option | Description |
| ------ | ----------- |
| `lat` | The latitude of your location<br>**Type:** `integer`<br>**Example:** `20.545`<br>**Default value:** `41.657` <br>|
| `lon` | The longitude of your location<br>**Type:** `integer`<br>**Example:** `-67.420`<br>**Default value:** `91.534` <br>|
| `timezone` | Your timezone in TZ database format<br>**Type:** `string` <br>**Example:** `Europe/Paris` <br>**Default value:** `America/Chicago`<br>**Note:** You can find a [list of all TZ timezones here.](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones)