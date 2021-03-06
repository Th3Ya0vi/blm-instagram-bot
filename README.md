# blm-instagram-bot
 Instagram bot that informs users using the BlackLivesMatter tag to post solid images that they may be accidentally hiding important information about the movement.
![Demonstration 1](https://i.imgur.com/cbW2vEY.png)
![Demonstration 2](https://i.imgur.com/nsYbHJl.png)

Uses a Google Cloud Function called [blm-cloud-function](https://github.com/char/blm-cloud-function) to determine if the image is a solid black image. This is to offload the image processing to the cloud and hopefully keep things running smooth.

## To-Do
1. Poll the tag. Right now it only goes through the current posts.
2. Keep a cache of posts the bot has already commented on.
3. Use multiple accounts to rotate and avoid being rate limited by Instagram.
4. Use a better way to detect solid images (Currently just checks if all RGB values are under 20)

Make sure to rename .env.example to .env