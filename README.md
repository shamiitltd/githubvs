![githubvs](https://raw.githubusercontent.com/shamiitltd/githubvs/master/resources/images/logo.svg)

# githubvs

One second to read GitHub code with VS Code.

## Usage

Just add `1s` after `github` and press `Enter` in the browser address bar for any repository you want to read.

For example, try it on the VS Code repo:

[https://githubvs.com/microsoft/vscode](https://githubvs.com/microsoft/vscode)

![VS Code - githubvs](https://raw.githubusercontent.com/shamiitltd/githubvs/master/resources/images/vs-code-githubvs.png)

You can also use [https://gitlab1s.com](https://gitlab1s.com) or [https://npmjs1s.com](https://npmjs1s.com) in the same way.

For browser extensions, see [Third-party Related Projects](https://github.com/shamiitltd/githubvs#third-party-related-projects).

Or save the following code snippet as a bookmarklet, you can use it to quickly switch between github.com and githubvs.com (GitHub markdown doesn't allow js links, so just copy it into a bookmark).

```
javascript: window.location.href = window.location.href.replace(/github(1s)?.com/, function(match, p1) { return p1 ? 'github.com' : 'githubvs.com' })
```

### Develop in the cloud

To edit files, run Docker containers, create pull requests and more, click the "Develop your project on [Gitpod](https://www.gitpod.io)" button in the status bar. You can also open the Command Palette (default shortcut `Ctrl+Shift+P`) and choose `githubvs: Edit files in Gitpod`.

![Gitpod Status Bar](https://raw.githubusercontent.com/shamiitltd/githubvs/master/resources/images/gitpod-statusbar.png)

## Documentation

- [How it works](https://github.com/shamiitltd/githubvs/blob/master/docs/guide.md)
- [Roadmap](https://github.com/shamiitltd/githubvs/projects/1)

## Enabling Private Repositories

If you want to view non-public repositories, you need to add an OAuth token. The token is stored only in your browser, and only send to GitHub when fetching your repository's files. Click on the icon near the bottom of the left-hand row of icons, and the dialog box will prompt you for it, and even take you to your GitHub settings page to generate one, if needed.

<img height="500px" src="https://raw.githubusercontent.com/shamiitltd/githubvs/master/resources/images/auth-token.png" />

## Screenshots

![VS Code - githubvs](https://raw.githubusercontent.com/shamiitltd/githubvs/master/resources/images/githubvsDemo1.gif)

![VS Code - githubvs](https://raw.githubusercontent.com/shamiitltd/githubvs/master/resources/images/demo.png)

## Development

### Cloud-based development

You can start an online development environment with [Gitpod](https://www.gitpod.io) by clicking the following button:

[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/shamiitltd/githubvs)

### Local development

```bash
git clone git@github.com:shamiitltd/githubvs.git
cd githubvs
yarn
yarn watch
# The cli will automatically open http://localhost:8080 once the build is completed.
# You can visit http://localhost:8080/shamiitltd/githubvs if it doesn't.
```

#### Local development with full VS Code build

You need [these prerequisites (the same ones as for VS Code)](https://github.com/microsoft/vscode/wiki/How-to-Contribute#prerequisites) for development with full VS Code build.
Please make sure you could build VS Code locally before the watch mode.

To verify the build:

```bash
cd githubvs
yarn build:vscode
```

After the initial successful build, you could use the watch mode:

```bash
cd githubvs
yarn
yarn watch-with-vscode
# The cli will automatically open http://localhost:8080 once the build is completed.
# You can visit http://localhost:8080/shamiitltd/githubvs if it doesn't.
```

### ... or ... VS Code + Docker Development

You can use the VS Code plugin [Remote-Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) `Dev Container` to use a Docker container as a development environment.

1. Install the Remote-Containers plugin in VS Code & Docker
2. Open the Command Palette (default shortcut `Ctrl+Shift+P`) and choose `Remote-Containers: Clone Repository in Container Volume...`
3. Enter the repo, in this case `https://github.com/shamiitltd/githubvs.git` or your forked repo
4. Pick either, `Create a unique volume` or `Create a new volume`

   - Now VS Code will create the docker container and connect to the new container so you can use this as a fully setup environment!

5. Open a new VS Code Terminal, then you can run the `yarn` commands listed above.

```bash
yarn
yarn watch
# The cli will automatically open http://localhost:8080 once the build is completed.
# You can visit http://localhost:8080/shamiitltd/githubvs if it doesn't.
```

### Format all codes

```bash
yarn format
```

It uses `prettier` to format all possible codes.

## Build

```bash
yarn
yarn build
```

## Feedback

- If something is not working, [create an issue](https://github.com/shamiitltd/githubvs/issues/new)

## Sponsors

The continued development and maintenance of githubvs is made possible by these generous sponsors:

<table><tbody><tr>
<td><a href="https://sourcegraph.com/">
<img height="40px" src="https://raw.githubusercontent.com/shamiitltd/githubvs/master/resources/images/sourcegraph-logo.svg">
</a></td>
<td><a href="https://vercel.com/?utm_source=vscode-githubvs&utm_campaign=oss">
<img height="40px" src="https://raw.githubusercontent.com/shamiitltd/githubvs/master/resources/images/vercel-logo.svg">
</a></td>
</tr></tbody></table>

## Partners

We are partnered with [OSS Insight](https://ossinsight.io/?utm_source=githubvs&utm_medium=github&utm_campaign=ghtrending) to get the Trending Repositories & some more Interesting Analytics. [OSS Insight](https://ossinsight.io/?utm_source=githubvs&utm_medium=github&utm_campaign=ghtrending) provides deep insights into GitHub repos, developers, and curated repo lists from billions of GitHub events. It’s built with [TiDB Cloud](https://www.pingcap.com/tidb-cloud/?utm_source=githubvs&utm_medium=github&utm_campaign=ghtrending).

<table><tbody><tr>
<td><a href="https://ossinsight.io/?utm_source=githubvs&utm_medium=github&utm_campaign=ghtrending">
<img height="40px" src="./resources/images/ossinsight-brand-dark.png">
</a></td>
</tr></tbody></table>

## Maintainers! :blush:

<table>
  <tbody><tr>
    <td align="center"><a href="https://github.com/shamiitltd"><img alt="" src="https://avatars.githubusercontent.com/shamiitltd" width="100px;"><br><sub><b>netcon</b></sub></a><br><a href="https://github.com/shamiitltd/githubvs/commits?author=shamiitltd" title="Code">💻 🖋</a></td> </a></td>
    <td align="center"><a href="https://github.com/xcv58"><img alt="" src="https://avatars.githubusercontent.com/xcv58" width="100px;"><br><sub><b>xcv58</b></sub></a><br><a href="https://github.com/shamiitltd/githubvs/commits?author=xcv58" title="Code">💻 🖋</a></td></a></td>
    <td align="center"><a href="https://github.com/Siddhant-K-code"><img alt="" src="https://avatars.githubusercontent.com/Siddhant-K-code" width="100px;"><br><sub><b>Siddhant Khare</b></sub></a><br><a href="https://github.com/shamiitltd/githubvs/commits?author=Siddhant-K-code" title="Code">💻 🖋</a></td> </a></td>
  </tr>
</tbody></table>

## Stargazers over time

[![Stargazers over time](https://api.star-history.com/svg?repos=shamiitltd/githubvs&type=Date)](https://star-history.com/#shamiitltd/githubvs&Date)

<details>
<summary>Third-party Related Projects</summary>
<br>

### Chrome Extensions

- [Repositree](https://chrome.google.com/webstore/detail/repositree/lafjldoccjnjlcmdhmniholdpjkbgajo) ([chouglesaud/repositree](https://github.com/chouglesaud/repositree))
- [github-code-viewer](https://chrome.google.com/webstore/detail/github-code-viewer/ecddapgifccgblebfibdgkagfbdagjfn) ([febaoshan/edge-extensions-github-code-viewer](https://github.com/febaoshan/edge-extensions-github-code-viewer))
- githubvs Extension ([Darkempire78/githubvs-Extension](https://github.com/Darkempire78/githubvs-Extension))
- [Github Web IDE](https://chrome.google.com/webstore/detail/adjiklnjodbiaioggfpbpkhbfcnhgkfe) ([zvizvi/Github-Web-IDE](https://github.com/zvizvi/Github-Web-IDE))
- [shortcut to githubvs](https://chrome.google.com/webstore/detail/shortcut-to-githubvs/gfcdbodapcbfckbfpmgeldfkkgjknceo) ([katsuhisa91/githubvs-shortcut](https://github.com/katsuhisa91/githubvs-shortcut))
- [githubvs Shortut - Open source](https://github.com/Fauzdar1/githubvs)
- [⚡️ 1s to githubvs!](https://github.com/holazz/webext-githubvs)
- [githubvs Google Chrome Extensions](https://github.com/Lonely-Mr-zhang/github_1s_vscode)

### Firefox Extensions

- [Repositree](https://addons.mozilla.org/en-US/firefox/addon/repositree/) ([chouglesaud/repositree](https://github.com/chouglesaud/repositree))
- [githubvs Extension](https://addons.mozilla.org/firefox/addon/githubvs-extension) ([Darkempire78/githubvs-Extension](https://github.com/Darkempire78/githubvs-Extension))
- [githubvs](https://addons.mozilla.org/firefox/addon/githubvs/) ([mcherifi/githubvs-firefox-addon](https://github.com/mcherifi/githubvs-firefox-addon))
- [Github Web IDE](https://addons.mozilla.org/firefox/addon/github-web-ide/) ([zvizvi/Github-Web-IDE](https://github.com/zvizvi/Github-Web-IDE))

### Microsoft Edge Extensions

- [github-code-viewer](https://microsoftedge.microsoft.com/addons/detail/githubcodeviewer/jaaaapanahkknbgdbglnlchbjfhhjlpi) ([febaoshan/edge-extensions-github-code-viewer](https://github.com/febaoshan/edge-extensions-github-code-viewer))
- [Github Web IDE](https://microsoftedge.microsoft.com/addons/detail/akjbkjciknacicbnkfjbnlaeednpadcf) ([zvizvi/Github-Web-IDE](https://github.com/zvizvi/Github-Web-IDE))

### Safari Extension

- [githubvs-For-Safari-Extension](https://apps.apple.com/us/app/readcodeonline/id1569026520?mt=12) ([code4you2021/githubvs-For-Safari-Extension](https://github.com/code4you2021/githubvs-For-Safari-Extension))

### Tampermonkey scripts

- [Mr-B0b/TamperMonkeyScripts/vscode.js](https://github.com/Mr-B0b/TamperMonkeyScripts/blob/main/vscode.js)
</details>
