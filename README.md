# Stuff you should know
## Objective
This objective of this project is to provide a list of basic development concepts geared towards beginning developers. These are listed below.
I have also included some other useful resources, such as - common command line commands, issue templates, website checklist and more. Those are presented as additional files in this repo. 
## Contribute
Feel free to contribute. Create a pull request, or shoot me an email at sb@sbarkin.com.
## Tooling
1. [CLI](https://en.wikipedia.org/wiki/Command-line_interface) (SSH Client)
   - [iTerm2](https://www.iterm2.com/) (Mac)
   - [Putty](https://www.putty.org/) (Windows)
   - [Linux Bash Shell](https://www.howtogeek.com/249966/how-to-install-and-use-the-linux-bash-shell-on-windows-10/) on Windows 10
   - Many others are available - if you are working with Linux servers it's best to find a something more native to Linux. One example is -  [Babun](http://babun.github.io/) 
1. FTP/SFTP
   - SFTP uses SSH credentials to connect
   - FTP uses FTP  credentials to connect (not secure)
   - [FileZilla](https://filezilla-project.org/)
   - [WinSCP](https://winscp.net/eng/index.php) (Windows)
1. Editors
   - [Atom](https://atom.io/)
   - [Sublime](https://www.sublimetext.com/) (Mac)
   - [Brackets](http://brackets.io/)
   - [Visual Studio Code](https://code.visualstudio.com/)
   - [Notepad++](https://notepad-plus-plus.org/) (Windows)
1. IDE
   - [JetBrains](https://www.jetbrains.com/) (multiple IDEs for many languages) 
   - [Visual Studio](https://visualstudio.microsoft.com/) 
   - [Eclipse](https://www.eclipse.org/ide/) (Mac)
   - [Xcode](https://developer.apple.com/xcode/) (Mac)
1. App Installer 
   - [Homebrew](https://brew.sh/) (Mac)
     - [Homebrew Cask](https://github.com/Homebrew/homebrew-cask)
   - [Ninite](Ninite.com) (Windows)
     - Safe Download of popular free software. Free software is often available on shady sites with bloatware or malware. Always make sure you are downloading from a trusted source. 
   - [macapps](https://macapps.link/en) (Mac)
   - [GetMacApps](http://www.getmacapps.com/) (Mac)
1. Sharing screenshots (no, don't take a picture of your screen with your camera :)
   - [Chrome extensions](https://chrome.google.com/webstore/search/screenshot?utm_source=chrome-ntp-icon&_category=extensions)
   - [Jing](https://www.techsmith.com/jing-tool.html)
   - [Gyazo](https://gyazo.com/)
   - [CloudApp](https://www.getcloudapp.com/)
   - [LightShot](https://prnt.sc/) ([see this extension too](https://chrome.google.com/webstore/detail/no-more-lightshot-ads/fiefoaeemgdpplhofbhkdehoidoajfld?utm_source=chrome-ntp-icon))
1. Issue Tracker
   - [Jira](https://www.atlassian.com/software/jira) - the leading option  
   - [YouTrack](https://www.jetbrains.com/youtrack/) - simpler and cheaper and usually sufficient alternative 
1. Time tracking
   - [toggle](toggl.com)
   - [Harvest](https://www.getharvest.com/)  
1. Chat Tools 
   - [Slack](https://slack.com/)
   - [Skype](https://www.skype.com/)
   - Google Hangouts
1. Email Options
   - [G Suite](https://gsuite.google.com/)
   - [Office 365](https://www.office.com/)
   - Self Hosted  
## Build
1. Setting up a local development environment 
   - Localhost web server
   - [XAMPP](https://www.apachefriends.org/index.html) and [WampServer](http://www.wampserver.com/en/) (Windows)
   - Virtual machine
        - [Vagrant](https://www.vagrantup.com/)
        - [VirtualBox](https://www.virtualbox.org/)
   - Package manager
     - NPM for JS, Composer for PHP, RubyGems for Ruby, Cocoa Pods for iOS, Nuget for C#
1. VCS ([version control](https://en.wikipedia.org/wiki/Version_control))
   - GIT
   - Common commands  `git add`, `git commit -m <msg>`, `git push`, `git pull`, `git status`
   - You should know how to initiate a remote repository connect to cloud hosted repo and how to clone a project
   - Understand  the [different  workflows](https://www.atlassian.com/git/tutorials/comparing-workflows), ie feature branches
1. Cloud GIT repositories
   - [GitHub](https://github.com/)
   - [BitBucket](https://bitbucket.org)
   - [GitLab](https://about.gitlab.com/)
1. [Semantic Versioning](https://semver.org/)
   - The most popular way of version numbering in software development
1. [SSH](https://en.wikipedia.org/wiki/Secure_Shell) /FTP/SFTP
1. Command line
   - Windows - command prompt, Mac- terminal
   - Common commands: `cd`, `mkdir`, `ls` (Unix)/`dir` (PC), `chmod` (unix),`vi`/`cat` (Unix)...
1. Popular JS Frameworks
   - React, Angular, Node.js, Vue.js
1. Content management systems (CMS) - sometimes used for web development
   - Drupal, WordPress, Joomla
1. [Postman](https://www.getpostman.com/) - for testing APIs    
## Deploy
1. CD/CI
   - Continuous integration
     - [Jenkins](https://jenkins.io/)
     - [Travis](https://travis-ci.com/)
   - Continuous deployment (or delivery)
1. Server environments
   - Development
   - Testing/staging/UAT (there may be multiple levels)
   - Production  
1. Server OS 
   - Windows Server - web server = ISIS 
   - Linux - Used for PHP and other technologies 
1. Web Servers 
   - Windows - IIS (used for .NET projects)
   - Apache
   - Nginx - the new kid on the block
1. [SSL](https://en.wikipedia.org/wiki/Transport_Layer_Security)
   - Encrypts traffic on a website 
   - [Let’s Encrypt](https://letsencrypt.org/) - free SSL
1. [IP Address](https://en.wikipedia.org/wiki/IP_address)
   - [IPv4](https://en.wikipedia.org/wiki/IPv4)
   - [IPv6](https://en.wikipedia.org/wiki/IPv6)
1. [DNS](https://en.wikipedia.org/wiki/Domain_Name_System)
   - Name servers
   - DNS records
   - MX records 
   - CNAME records 
1. [CDN](https://en.wikipedia.org/wiki/Content_delivery_network)
   - [Cloudflare](https://www.cloudflare.com/)
1. Cloud Hosting Companies
   - [AWS](https://aws.amazon.com/)
   - [Azure](https://azure.microsoft.com/en-us/)
   - [Google Cloud](https://cloud.google.com/)
   - [DigitalOcean](https://www.digitalocean.com/)
1. Container Management
   - [Docker](https://www.docker.com/)
   - [Kubernetes](https://kubernetes.io/)
1. Serverless, Headless CMS, [AMP](https://www.ampproject.org/)
## Monitor 
1. [FullStory](https://www.fullstory.com/), [HotJar](https://www.hotjar.com/), [Google Analytics](https://analytics.google.com/analytics/web/)
## Resources 
- Got a question?
   - Ask Google
- Still can find the answer?
   -  Ask on [StackExchange](https://stackexchange.com/)
- [Git Cheat sheet](https://services.github.com/on-demand/downloads/github-git-cheat-sheet.pdf)
## Random Terms 
   - Client - a program on the computer used to access something. Email client, CLI client...
   - Provision (server)
## Design 
1. UI/UX 
   - Design
     - [Sketch](https://www.sketchapp.com/) (Mac)
     - [Adobe XD](https://www.adobe.com/products/xd.html)
     - [Framer](https://framer.com/)
     - [InVision Studio](https://www.invisionapp.com/studio)
     - [Figma](https://www.figma.com/)
   - Prototype/Share
     - [InVision](https://www.invisionapp.com/)
     - [Sketch Cloud](https://www.sketchapp.com/)
     - [Marvel](https://marvelapp.com/)
   - Handoff
     - [Zeplin](https://zeplin.io/)
     - [InVision Inspect](https://www.invisionapp.com/feature/inspect/)
   - DSM (Design system management)
     - Style Guide
     - [InVision DSM](https://www.invisionapp.com/design-system-manager/learn)
     - Sketch Libraries
1. General Design
   - Illustrator - primarily for vector images (free alternative [Inkscape](https://inkscape.org/))
   - Photoshop - primarily for raster (free alternative GIMP)
   - Grab a color value from your screen - http://colorcop.net/  (Windows)
1. Image types (which to use when)
   - jpeg - for complex images with many colors (e.g. lifestyle image)
   - png - with transparency (e.g. logo image)
   - svg - vector image format 
1. Raster vs vector
1. Need inspiration? Go to [Dribbble](https://dribbble.com/) 
## Setting up your computer 
1. Windows account types
   - AD
   - Local
   - Windows Account
1. Pinning to doc/taskbar
1. Chrome
   - Signing into chrome 
   - Bookmarks (Bookmarks bar, folders)
   - Ad blocker - [uBlock Origin](https://chrome.google.com/webstore/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm?utm_source=chrome-ntp-icon)
   - Password Manager - [Lastpass](https://chrome.google.com/webstore/detail/lastpass-free-password-ma/hdokiejnpimakedhajhdlcegeplioahd?utm_source=chrome-ntp-icon)
1. Split Windows 
## General Computer Terms/Concepts
1. Keyboard shortcuts (Mac/Windows)
   - Command/Ctrl + C,  copy
   - Command/Ctrl + V, paste
   - Command/Ctrl + X, cut (Does not work in Finder)
1. Browser Shortcuts (Mac/Windows)
   - Command/Ctrl + R,  refresh page
   - Command/Ctrl + Shift+ R,  hard refresh