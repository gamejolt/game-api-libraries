> Collection of community libraries for the Game Jolt Game API. Help contribute!

## To add a new library

- Clone this repo and make a branch.
- Add a new JSON file named based on what you call your library. Please slugify it by lowercasing and putting hyphens instead of spaces.
- Make a pull request on Github with this new file.

## To update a library

- Make a pull request with the changes you'd like to make.

## JSON file format

```json
{
	"name": "Unity API",
	"api": "1.2",
	"engine": "Unity",
	"homepage": "http://gamejolt.com/games/unity-api/15887",
	"author": "loicteixeira",
	"code": "https://github.com/loicteixeira/gj-unity-api",
	"bugs": "https://github.com/loicteixeira/gj-unity-api/issues",
	"license": "MIT"
}
```

Please use single tabs instead of spaces in your JSON file.

- `name` **required** can be anything. Call it what you'd like.
- `api` **required** a version string that matches the Game API version that your library implements.
- `engine` **required** the programming language that your library works in, or the game engine/tool.
- `homepage` **required** a URL where you can find more information on the library, and to download/get it.
- `author` **required** either a single Game Jolt username, or an array of usernames.
- `code` **optional** a URL where you can view the code for your library.
- `bugs` **optional** a URL for where users can issue bugs for your library.
- `license` **required** what you have licensed your library under: MIT, GPLv3, etc.

