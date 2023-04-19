<img src="https://user-images.githubusercontent.com/74150746/233064892-0fe1e1b4-c1fa-4edd-8405-d742b10123a0.png" align="center"/>

<h1>1. Getting started</h1>

Before cloning and building make sure that:
```
- you aren't using macOS,
- you are running 64-bit,
- you are running latest "your unix-like distro" version,
- you have more than 16 GB of RAM, 350 GB of SSD/HDD
```

<h2>2. Setting up a build environment</h2>

2.1. Installing dependencies
```
sudo apt-get install git-core gnupg flex bison build-essential zip curl zlib1g-dev libc6-dev-i386 libncurses5 \
lib32ncurses5-dev x11proto-core-dev libx11-dev lib32z1-dev libgl1-mesa-dev libxml2-utils xsltproc unzip fontconfig
```

2.2. Installing Repo
```
mkdir -p ~/.bin && PATH="${HOME}/.bin:${PATH}" && curl https://storage.googleapis.com/git-repo-downloads/repo > ~/.bin/repo && chmod a+rx ~/.bin/repo
```

<h2>3. Initializing toontown</h2>

3.1. Creating working directory
```
cd ~ && mkdir toontown && cd toontown
```

3.2. Initializing manifest in working directory
```
repo init https://github.com/toontownAOSP/platform_manifest.git -b tofu
```

3.3. Syncing sources
```
repo sync
```

<h2>4. Contributions</h2>

To submit changes/patches - send PRs on GitHub.
