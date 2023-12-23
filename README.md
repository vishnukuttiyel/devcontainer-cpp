# Devcontainer-cpp Setup Guide

## Overview

This guide provides instructions for setting up the development environment for `devcontainer-cpp` on Windows using Docker. The steps also include optional instructions for setting up XServer for GUI visualization.

## Setup Steps

### 1. Install Docker

Follow the [official Docker installation guide](https://docs.docker.com/desktop/install/windows-install/) to install Docker on your Windows machine.

### 2. Install Visual Studio Code

- Install Visual Studio Code.
- Install the Remote Development extension.
- Open VSCode, press `Ctrl + Shift + P`, type 'dev containers: Clone Repository in Container Volume,' and clone this repository.
- Allow some time for the download and installation of the container.

## Optional: Setting up XServer

If you want to visualize the GUI from Docker in Windows, follow the steps in [this YouTube tutorial](https://www.youtube.com/watch?v=BDilFZ9C9mw) to set up XServer. Ensure you have XServer installed.

## Running the Application

To run the application, execute the following commands in the terminal:

```bash
mkdir build
cd build
cmake ..
make
./bin/sfml-app
