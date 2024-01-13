<div align="center" width="100%">
    <img src="./public/icon.svg" width="128" alt="" />
</div>

# Uptime | Niansuh

Uptime | Niansuh is an easy-to-use self-hosted monitoring tool.


<img src="https://github.com/Niansuh/uptime/assets/139365289/2b248c3b-4407-4a26-8ee5-8b825f7ed367" width="700" alt="" />


## ⭐ Features

- Monitoring uptime for HTTP(s) / TCP / HTTP(s) Keyword / HTTP(s) Json Query / Ping / DNS Record / Push / Steam Game Server / Docker Containers
- Fancy, Reactive, Fast UI/UX
- Notifications via Telegram, Discord, Gotify, Slack, Pushover, Email (SMTP), and [90+ notification services, click here for the full list](https://github.com/niansuh/uptime/tree/master/src/components/notifications)
- 20-second intervals
- [Multi Languages](https://github.com/niansuh/uptime/tree/master/src/lang)
- Multiple status pages
- Map status pages to specific domains
- Ping chart
- Certificate info
- Proxy support
- 2FA support

## 🔧 How to Install

### 🐳 Docker

```bash
docker run -d --restart=always -p 3001:3001 -v uptime-kuma:/app/data --name uptime-kuma niansuh/uptime-kuma:1
```

Uptime Kuma is now running on http://localhost:3001

> [!WARNING]
> File Systems like **NFS** (Network File System) are **NOT** supported. Please map to a local directory or volume.

### 💪🏻 Non-Docker

Requirements:

- Platform
  - ✅ Major Linux distros such as Debian, Ubuntu, CentOS, Fedora and ArchLinux etc.
  - ✅ Windows 10 (x64), Windows Server 2012 R2 (x64) or higher
  - ❌ Replit / Heroku
- [Node.js](https://nodejs.org/en/download/) 14 / 16 / 18 / 20.4
- [npm](https://docs.npmjs.com/cli/) 9
- [Git](https://git-scm.com/downloads)
- [pm2](https://pm2.keymetrics.io/) - For running Uptime Kuma in the background

```bash
# Update your npm
npm install npm@9 -g

git clone https://github.com/niansuh/uptime.git
cd uptime-kuma
npm run setup

# Option 1. Try it
node server/server.js

# (Recommended) Option 2. Run in the background using PM2
# Install PM2 if you don't have it:
npm install pm2 -g && pm2 install pm2-logrotate

# Start Server
pm2 start server/server.js --name uptime
```

Uptime Kuma is now running on http://localhost:3001

More useful PM2 Commands

```bash
# If you want to see the current console output
pm2 monit

# If you want to add it to startup
pm2 save && pm2 startup
```

### Advanced Installation

If you need more options or need to browse via a reverse proxy, please read:

https://github.com/niansuh/uptime-kuma/wiki/%F0%9F%94%A7-How-to-Install

## 🆙 How to Update

Please read:

https://github.com/niansuh/uptime-kuma/wiki/%F0%9F%86%99-How-to-Update

## 🆕 What's Next?

I will assign requests/issues to the next milestone.

https://github.com/niansuh/uptime-kuma/milestones

## ❤️ Sponsors

Thank you so much! (GitHub Sponsors will be updated manually. OpenCollective sponsors will be updated automatically, the list will be cached by GitHub though. It may need some time to be updated)

<img src="https://uptime.kuma.pet/sponsors?v=6" alt />

## 🖼 More Screenshots

Light Mode:

<img src="https://uptime.kuma.pet/img/light.jpg" width="512" alt="" />

Status Page:

<img src="https://user-images.githubusercontent.com/1336778/134628766-a3fe0981-0926-4285-ab46-891a21c3e4cb.png" width="512" alt="" />

Settings Page:

<img src="https://niansuh.net/uptimekuma/2.jpg" width="400" alt="" />

Telegram Notification Sample:

<img src="https://niansuh.net/uptimekuma/3.jpg" width="400" alt="" />

## Motivation

- I was looking for a self-hosted monitoring tool like "Uptime Robot", but it is hard to find a suitable one. One of the closest ones is statping. Unfortunately, it is not stable and no longer maintained.
- Wanted to build a fancy UI.
- Learn Vue 3 and vite.js.
- Show the power of Bootstrap 5.
- Try to use WebSocket with SPA instead of a REST API.
- Deploy my first Docker image to Docker Hub.

If you love this project, please consider giving it a ⭐.

## 🗣️ Discussion / Ask for Help

⚠️ For any general or technical questions, please don't send me an email, as I am unable to provide support in that manner. I will not respond if you ask questions there.

I recommend using Google, GitHub Issues, or Uptime Kuma's subreddit for finding answers to your question. If you cannot find the information you need, feel free to ask:

- [GitHub Issues](https://github.com/niansuh/uptime-kuma/issues)
- [Subreddit (r/UptimeKuma)](https://www.reddit.com/r/UptimeKuma/)

My Reddit account: [u/niansuhlam](https://reddit.com/u/niansuhlam)
You can mention me if you ask a question on the subreddit.

## Contributions

### Create Pull Requests

We DO NOT accept all types of pull requests and do not want to waste your time. Please be sure that you have read and follow pull request rules:
[CONTRIBUTING.md#can-i-create-a-pull-request-for-uptime-kuma](https://github.com/niansuh/uptime-kuma/blob/master/CONTRIBUTING.md#can-i-create-a-pull-request-for-uptime-kuma)

### Test Pull Requests

There are a lot of pull requests right now, but I don't have time to test them all.

If you want to help, you can check this:
https://github.com/niansuh/uptime-kuma/wiki/Test-Pull-Requests

### Test Beta Version

Check out the latest beta release here: https://github.com/niansuh/uptime-kuma/releases

### Bug Reports / Feature Requests

If you want to report a bug or request a new feature, feel free to open a [new issue](https://github.com/niansuh/uptime-kuma/issues).

### Translations

If you want to translate Uptime Kuma into your language, please visit [Weblate Readme](https://github.com/niansuh/uptime-kuma/blob/master/src/lang/README.md).

### Spelling & Grammar

Feel free to correct the grammar in the documentation or code.
My mother language is not English and my grammar is not that great.


