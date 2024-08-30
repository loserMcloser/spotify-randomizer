# spotify-randomizer

## Description
Simple spotipy python script to randomize a spotify playlist.

## Dependencies
* [spotipy](https://pypi.org/project/spotipy/)
* [PyYAML](https://pypi.org/project/PyYAML/)
* [platformdirs](https://pypi.org/project/platformdirs/)

## Setup
1. Create a Spotify application so you can use the spotipy backend.
You can do this at the [Spotify developer website](https://developer.spotify.com/dashboard).
1. Enter the newly-created spotify application's client ID and secret into `config.yaml`.
1. In the "Redirect URIs" field of your spotify application's settings
(still on the Spotify developer website),
add `http://localhost:PORT` with PORT replaced by either the default value `14523` or by a port number of your choosing.
Enter your port number as the value of `redirect_uri_port` in `config.yaml`.
1. Continue editing `config.yaml` (instructions within).
You may omit the `playlists` setting if you wish,
and the script will prompt you to choose a playlist to randomize.
1. Create a directory called `spotify-randomizer` under the `config` directory of your user account on your system.
(On Linux: `mkdir ${XDG_CONFIG_HOME}/spotify-randomizer`.)
Then save `config.yaml` under this directory.
(If you are not sure where to create this directory, run the script without any `config.yaml` and it will tell you where you need to put it.)

Once this is done you are ready to run the `spotify-randomizer` script.
