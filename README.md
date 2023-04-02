# Spotify Playlist Downloader

Download songs from Billboard 100 based on the selected Year from user.

# Tell me more!

I want an easy way to create a new playlist based on the selected year so that I don't have to add the songs manually. It picks up the metadata from Spotify API and [Spotipy](https://spotipy.readthedocs.io/en/2.22.1/) to search and add the songs by title.

It will create a new playlist and add all the found songs into the new playlist.

# Running

Install using pip
  pip3 install spotipy
Get the CLIENT_ID & CLIENT_SECRET from Spotify
  Create a sp Client
  sp = spotipy.Spotify(
  auth_manager=SpotifyOAuth(
  scope="playlist-modify-private",
  redirect_uri="https://open.spotify.com/",
  client_id=CLIENT_ID,
  client_secret=CLIENT_SECRET,
  show_dialog=True,
  cache_path="token.txt"
  )
  )
