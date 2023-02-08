Dockerfile is a file written in a specific format

- it is written in instructions and argument format
- Examples of instructions: FROM, RUN, COPY, ENTRYPOINT
- Everything on the right is an argument to those instructions

**Analyzing a Dockerfile**
- FROM Ubuntu <--- start from a base OS or another image-

**Install all dependencies**
- RUN apt-get update
- RUN apt-get install python
- RUN pip install flash
- RUN pip install flash-mysql 

- COPY . /opt/source-code <--- copy source code


**Layered Architecture**

When docker builds these, it does so in a layered architecture

Layer 1 - Base Ubuntu Layer

Layer 2 - Changes in apt packages

Layer 3 - Changes in pip packages

Layer 4 - Source code

Layer 5 - Update Entrypoint with "flask command"


**Run docker build command**

`docker build Dockerfile -t mmumshad/my-custom-app`

all the layers that are built are cached by docker

in case a particular step was to fail

re-running docker build command will re-use previous layers that are cached

**What can you containerize?**

you can containerize almost all the applications
