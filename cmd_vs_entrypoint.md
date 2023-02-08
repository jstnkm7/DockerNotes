##

I noticed CMD can be written in two ways:

- JSON array format

- regular bash command prompt style

And for entrypoints, I understand that...

- they are appended at docker run-time and we can apply our command-line argument and use the appended "entrypoint" command in bash. Ex: docker run centos 10

**IF both CMD and ENTRYPOINT are defined**

- CMD can pass default parameters to ENTRYPOINT if both are defined.
