# Nmap-Guide
More in-depth guide to the utility of Nmap
<!-- This is how you write notes in secret -->

Practicing pull requests in GitHub Desktop & Atom.io while accessing https://GitHub.com <!-- -->


<img style="display: block;-webkit-user-select: none;margin: auto;background-color: hsl(0, 0%, 90%);transition: background-color 300ms;" src="https://bestanimations.com/Computers/funny-computer-animated-gif-35.gif">

 <div id="top"></div>
 
<!--
*** Editor's notes:
## Describe
### Give examples
#### Display screen shots

-->

 </div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>


<!-- ABOUT THE PROJECT -->
<h1 align="center">
# So What Is Nmap ? ?

</h1>

<!-- PROJECT LOGO -->

![image](https://user-images.githubusercontent.com/104815254/170253876-10fbb2e0-2dc3-4fbb-86dc-5c4130fa0647.png)

Nmap (Network Mapper) is an open source tool for network discovery and security testing, originally published by Gordon "Fyodor" Lyon.
The official website is (http://nmap.org). Nmap is a free and open source (licensed) utility for network discovery and security testing.
Many network and system administrators also find it useful for tasks such as inventorying the network, managing service upgrade schedules,
and monitoring server or service availability.
 Nmap uses raw IP packets in new ways to identify which servers are available on the network, what services (application names and versions)
 these servers provide, the operating system (and OS version) they provide. operating system) they are running, the type of packet
 filter/firewall used, and dozens of other features. It is designed for fast scanning of large networks, but works well on single servers.
 Nmap runs on all major computer operating systems, and official binaries are available for Linux, Windows, and Mac OS X.


<h1 align="center"> # Installation of Nmap
</h1>
 
Nmap has great support for different environments.

Windows: Install from the official site http://nmap.org For Windows, both GUI and command line options are available. The GUI option for Nmap is Zenmap.

Linux (Ubuntu and Debian): Fire the command in the Linux terminal: apt-get install nmap

In the below image, I have already installed Nmap.



![image](https://user-images.githubusercontent.com/104815254/170257189-07659ac4-278d-4440-b0f7-f97dfbf1f0b4.png)


Introduction to NMAP
Nmap is an open source port scanning tool that was first published in September 1997. The source code was
posted in an article in Phrack Magazine, and it was further developed by the community. The latest release,
as of this post date, is Nmap 7.92, released in August 2021.

Nmap is the cornerstone of the recon phase for network 
security testing, and for good reason, it comes with a
library of Lua scripts that add a lot of utility. There 
are scripts for everything from scanning for
vulnerabilities to conducting brute force attacks. 
These scripts are all handled by the Nmap Scripting 
Engine (NSE), and we will go over that
once we’ve dialed in on some of the basics.


As always during reconnaissance, scanning is the initial stage for information gathering.

## What is reconnaissance?

Reconnaissance is to collect as much as information about a target network as possible.From a hacker’s 
perspective, the information gathered is very helpful to make an attack, so to block that type of malicious 
attempt, generally a penetration tester tries to find the information and to patch the vulnerabilities if found. 
This is also called Footprinting. Usually by information gathering, someone can find the below information:

E-mail Address
Port no/Protocols
OS details
Services Running
Traceroute information/DNS information
Firewall Identification and evasion
And many more…



So for information gathering, scanning is the first part.
For scanning, Nmap is a great tool for discovering Open ports, 
protocol numbers, OS details, firewall details, etc.




Before we can understand Nmap we have to understand port scanning.
Computers communicate using ports. There are a total of 65,535 ports, 
but few of these ports will be utilized yet alone open.

Within these large number of ports, there are whats known as common or 
well-known ports which range from 0 to 1023. Here are some examples:

<ul><li>port 20 (FTP)
  </li><li>port 22 (SSH/SCP)
  </li><li>port 23 (Telnet)
  </li><li>port 53 (DNS)
  </li><li>port 80 (HTTP)
  </li><li>port 443 (HTTPS)
  </li></ul>




Here's why:
* Your time should be focused on creating something amazing. A project that solves a problem and helps others
* You shouldn't be doing the same tasks over and over like creating a README from scratch
* You should implement DRY principles to the rest of your life :smile:

Of course, no one template will serve all projects since your needs may be different. So I'll be adding more in the near future. You may also suggest changes by forking this repo and creating a pull request or opening an issue. Thanks to all the people have contributed to expanding this template!

Use the `BLANK_README.md` to get started.

<p align="right">(<a href="#top">back to top</a>)</p>



# Built With

This section should list any major frameworks/libraries used to bootstrap your project. Leave any add-ons/plugins for the acknowledgements section. Here are a few examples.

* [Kali.js](https://kali.org/)
* [Nmap.js](https://nmap.org/)
* [Microsoft](https://microsoft.com/)
* [Java](https://java.com/en/)
* [Atom](https://atom.io/)
* [______](https://)
* [Bootstrap](https://getbootstrap)
* [JQuery](https://jquery.com)
* [Azure Portal]
* [Google Cloud Platform]
* [Amazon Web Services]

Equipment Powered

* CPU [AMD Ryzen 9](https://amd.com) (OC 5%)
* GPU [RTX 3060 (OC 22%)]
* RAM [16gb (Expandable to 40gb)]
* OS [Windows 11 / Linux Kali]
* VM [Oracle VM VirtualBox; Kali Linux & Parrot]
* 



<p align="right">(<a href="#top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.

### Prerequisites

This is an example of how to list things you need to use the software and how to install them.
* npm
  ```sh
  npm install npm@latest -g
  ```

### Installation

_Below is an example of how you can instruct your audience on installing and setting up your app. This template doesn't rely on any external dependencies or services._

1. Get a free API Key at [https://example.com](https://example.com)
2. Clone the repo
   ```sh
   git clone https://github.com/your_username_/Project-Name.git
   ```
3. Install NPM packages
   ```sh
   npm install
   ```
4. Enter your API in `config.js`
   ```js
   const API_KEY = 'ENTER YOUR API';
   ```

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage

Use this space to show useful examples of how a project can be used. Additional screenshots, code examples and demos work well in this space. You may also link to more resources.

_For more examples, please refer to the [Documentation](https://example.com)_

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- ROADMAP -->
## Roadmap

- [x] Add Changelog
- [x] Add back to top links
- [ ] Add Additional Templates w/ Examples
- [ ] Add "components" document to easily copy & paste sections of the readme
- [ ] Multi-language Support
    - [ ] Chinese
    - [ ] Spanish

See the [open issues](https://github.com/othneildrew/Best-README-Template/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Your Name -  - John Smithh

Project Link: [https://github.com/testcomputer/Nmap-Guide](https://github.com/testcomputer/Nmap-Guide)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

Use this space to list resources you find helpful and would like to give credit to. I've included a few of my favorites to kick things off!

* [Choose an Open Source License](https://choosealicense.com)
* [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet)
* [Malven's Flexbox Cheatsheet](https://flexbox.malven.co/)
* [Malven's Grid Cheatsheet](https://grid.malven.co/)
* [Img Shields](https://shields.io)
* [GitHub Pages](https://pages.github.com)
* [Font Awesome](https://fontawesome.com)
* [React Icons](https://react-icons.github.io/react-icons/search)

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/othneildrew/Best-README-Template/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/othneildrew/Best-README-Template/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/othneildrew/Best-README-Template/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/othneildrew/Best-README-Template/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/othneildrew
[product-screenshot]: images/screenshot.png
- [Machine Learning for Beginners](https://aka.ms/ml-beginners)
- [IoT for Beginners](https://aka.ms/iot-beginners)
- [Data Science for Beginners](https://aka.ms/datascience-beginners)
- [AI for Beginners](https://aka.ms/ai-beginners)






 ## Contribution Guidelines
Thank you for your interest in contributing!

Please ensure your pull request adheres to the following guidelines:

- The purpose of this list is to increase the knowledge of testers and to discover new tools to help you on the way.
- This QA and Testing road map includes the most important skills and knowledge that you require to start a career with. NOT EVERY THING!
- You can use issues for requests/ improvements
- Feel free to provide a translated versions.
- Keep descriptions short and simple, but descriptive.
- End all descriptions with a full stop/period.
- Check your spelling and grammar.
- Make sure your text editor is set to remove trailing whitespace.
- When you issue a pull request, you agree that your contribution is in the public domain (guided by the CC0 license).
