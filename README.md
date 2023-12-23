# devcontainer-cpp

# How to set up the environment on windows
All info from this youtube video 'https://www.youtube.com/watch?v=SDa3v4Quj7Y&t=1521s'

- Install docker: 'https://docs.docker.com/desktop/install/windows-install/'
- Install vscode
  - Install remote development extension
  - ctrl + shift + p, type 'dev containers: Clone Repository in Container Volume' and clone this repo
  - Download and installation of container will take some time


# Follow youtube to setup xserver to visualise gui from docker in windows
`https://www.youtube.com/watch?v=BDilFZ9C9mw`
install xserver


To run the app. 

```console
mkdir build
cd build
cmake ..
make
./bin/sfml-app
```



