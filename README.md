# hot100-trends-pt2
Exploring trends in the Billboard Hot 100

## Setup

### Install dependencies

Install all dependencies from Pipfile:
```
pipenv install
```

If there are any errors, launch a virtual shell to use for running the programs:
```
pipenv shell
```

### Spotify credentials

Sign up for a Spotify Developer account and create a new app. Then, create a file named **.env** in the working directory.

In the **.env** file, create two new environment variables: **SPOTIPY_CLIENT_ID** and **SPOTIPY_CLIENT_SECRET**. Assign them to the Client ID and Client Secret ID found in your Spotify app. The file should look like this:
```
SPOTIPY_CLIENT_ID='abcde123456789'
SPOTIPY_CLIENT_SECRET='123456789abcde'
```

## Data format

### In `hot100files/`

| **Rank**           | **Title**         | **Artist(s)**     | **Artists separately**   |
|--------------------|-------------------|-------------------|--------------------------|
| Ranking in Hot 100 | Title of the song | Artists as listed | Artists separated by ';' |

