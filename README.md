# **OS Lab code written under the guidance of Sir Srinivasa T.M. and Sir Muneeshwaran P.**

Operating System built on top of XSM virtual string machine

---

## Getting Started (Docker required)

### 1. Clone the Repository

```bash
git clone https://github.com/farzanfaisal77/eXpOS
```

### 2. Navigate to the Project Folder

```bash
cd eXpOS
```

### 3. Build the Container Image

```bash
docker build -t expos:ubuntu20.04 .
```

### 4. Start a Container Instance

```bash
docker run -v $PWD/workdir:/home/expos/myexpos/workdir -d --name expos -i expos:ubuntu20.04
```

> This mounts the local `workdir` folder into the container so your files are accessible from both sides.

---

## Connecting to the Container

### Start the container (if not already running)

```bash
docker start expos
```

### Open a bash shell inside the container

```bash
docker exec -it expos /bin/bash
```

### Alternative: VS Code Dev Containers

If you use Visual Studio Code, you can attach directly to the running container using the **Dev Containers** extension — no terminal required.

<a href="https://exposnitc.github.io/Roadmap.html"> roadmap link</a>