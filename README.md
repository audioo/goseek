<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/audioo/goseek">
    <img src="./images/ico.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">GoSeek</h3>
  <p align=center>
    <a target="_blank" href="https://goreportcard.com/report/github.com/audioo/goseek" title="report"><img src="https://goreportcard.com/badge/github.com/audioo/goseek"></a>
    <a href="https://pkg.go.dev/github.com/audioo/goseek"><img src="https://pkg.go.dev/badge/github.com/audioo/goseek.svg" alt="Go Reference"></a>
    <a href="https://gitpod.io/#https://github.com/audioo/goseek"><img src="https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod"></a>
    <br>
    <a target="_blank" href="https://golang.org" title="Go version: 1.16"><img src="https://img.shields.io/badge/Golang-1.16-blue.svg?style=flat-square"></a>
    <a target="_blank" href="./LICENSE.md" title="LICENSE"><img src="https://img.shields.io/badge/License-Apache&#8208;2.0-blue.svg?style=flat-square"></a>
    <a target="_blank" href="mailto:hyperaudio@protonmail.com" title="EMAIL"><img src="https://img.shields.io/badge/Contact-Email-blue.svg?style=flat-square"></a>
    <a target="_blank" href="#" title="VERSION"><img src="https://img.shields.io/badge/Version-0.6.2-blue.svg?style=flat-square"></a>
  </p>
  <p align="center">
    OSINT & OPSEC Multi-Tool
    <br />
    <!-- <a href="https://github.com/othneildrew/Best-README-Template"><strong>Explore the docs »</strong></a> -->
    <br />
</p>



<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
    </li>
    <li><a href="#install-and-run">Install and Run</a></li>
    <li><a href="#running-with-docker">Running with Docker</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

<!--<img src="./images/disp.jpg"></img>-->

**I have always found Open-Source Intelligence and Operations Security to be intriguing. I started learning Golang in the beginning of February of 2021 and have been looking for new projects to help strengthen my knowledge. I also wanted these projects to keep me engaged over time and prove somewhat useful instead of making just another calculator. I hope to build on GoSeek and expand it's use cases in a way that others can benefit**

Features:

- [x] Username Lookup - Inspired by [Sherlock](https://github.com/sherlock-project/sherlock), includes account deletion sites.
- [x] IP Lookup - Uses [ip-api](https://ip-api.com/)
- [x] License Plate & VIN Lookup - Uses [htmlquery](https://github.com/antchfx/htmlquery)
- [x] Info Cull - Data narrowing using [gofpdf](https://github.com/jung-kurt/gofpdf), inspired by [HINTS](https://github.com/jadekeys/hints)
- [x] Fake Identity Generator - Name (male, female, or gender neutral), Location, Date of Birth, Username, and Password 

<!-- USAGE EXAMPLES -->
## Install and Run

Download via 'go get':
<code>go get -u github.com/audioo/goseek</code>

Run in terminal:
<code>goseek [command] [args]</code>

**OR**

Download via 'git clone':
<code>git clone https://github.com/audioo/goseek.git</code>

Navigate into GoSeek directory:
<code>cd goseek</code>

Run via 'go run': <code>go run main.go [command] [args]</code>
or build: <code>go build main.go</code>

## Running with Docker
1 - Build: <code>docker build -t goseek . </code>

2 - Run w/ Flags: <code>docker run --rm -it goseek [command] [args] . </code>

3 - Example: <code>docker run --rm -it goseek user audioo n .</code>

## Roadmap

- [x] Setup Username Lookup based on status code responses and optimize via goroutines
- [x] Setup IP Lookup
- [x] Setup re-write of HINTS (cull)
- [x] Setup License Plate to VIN conversion using htmlquery
- [x] Setup VIN Lookup using htmlquery
- [x] Setup fake identity generator (name, location, dob, username, password)
- [x] Switch to Cobra CLI
- [x] Implement Docker
- [x] Organize project structure
- [x] Setup Godoc base
- [ ] Accept more than just status code responses in Username Lookup
- [ ] Setup proper returns in Username Lookup for third-party applications
- [ ] Setup email lookup (site associations, breaches, etc...)
