# Public Spotify Liked Songs Playlist
A python program to automatically add your liked songs to a public spotify playlist. 

## Instructions
1. **Install Dependencies**
  
  **Make sure you have python downloaded. https://www.python.org/downloads/**

  Open your command prompt and type

  `pip install spotipy`

2. **Set up your `config.py` file.**

  ```
  client_id = "client-id-here"
  client_secret="client-secret-here"

  playlist_id = "playlist-id-here"
  ```

  You will get your client tokens from the spotify developer dashboard, (https://developer.spotify.com/dashboard/), **Be sure to add `http://localhost:8888/callback` as your redirect url in the Spotify Dev Dashboard**. Then you will get your playlist id from your
  desired playlist's song link. ` https://open.spotify.com/playlist/{YOUR-PLAYLIST-ID-HERE}?si=42o4uh40284y `

  ![image](https://user-images.githubusercontent.com/83687479/187978856-5410bc2f-a31c-4231-9443-7d076d116c67.png)

---

- **(OPTIONAL) Set up your file to be automatically ran on a given day of the week using batch files and Windows Task Scheduler.**

1. Create a text document in the folder you downloaded and write these into the first line. ```<Your Python.exe Location> <Your python Scripts Location>``` (filling those in with your personal locations)
2. Save that file as `yourfilename.bat`. Feel free to change "yourfilename" to whatever.
3. Click your windows button and search for "Windows Task Scheduler".
4. Click "Create Basic Task" on the top right.
5. Choose the Trigger Time.
6. Choose "Start a Program".
7. Locate the .bat file we created earlier.
8. Choose finish and you should be all set!

**If you dont want the cmd window popping up every time the script runs, go to the task's properties and make sure to choose `Run whether user is logged on or not`
and then check the `Do not store password` box.**
