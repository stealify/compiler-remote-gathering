# compiler-remote-gathering
A Tool which is part of the @stealify/compiler that gathers Project Information to consider next optimization steps.

## What does it do?
It offers a Remote Interface for the Stealify Compiler and allows him mainly to access your project files and your host process list it works without root
It is often part of diffrent other stealify compiler parts that need to retrive process or file information from a remote host.
It is importent to say that this is designed without Write Functionality it is not designed to modify files so it is a readonly concept.
It needs correct filesystem permissions and a single entrypoint directory that even can be a mono repo or a directory full of symlinks as long as it has
the needed permissions to read all needed files so running it as root will always work for everything.

## Why?
Mainly because the Stealify Compiler it self is a distributed compiler so it is clear that this system needs a way to audit files.
it needs to do that secure so this system is designed to use a strong pks for encryption and auth. 
