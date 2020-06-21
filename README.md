#BPF-Playground

Playground for using when we need `develop/play` on macOS.

## Usage

* We'll assume you've installed VirtualBox and Vagrant.

Setup the vagrant session (this will take a while).

```sh
make setup
```

Once vagrant session is up, you can verify your install using the the following script:

```sh
vagrant ssh
sudo /usr/share/bcc/tools/biolatency
```

```
usecs               : count     distribution
         0 -> 1          : 0        |                                        |
         2 -> 3          : 0        |                                        |
         4 -> 7          : 0        |                                        |
         8 -> 15         : 0        |                                        |
        16 -> 31         : 0        |                                        |
        32 -> 63         : 0        |                                        |
        64 -> 127        : 24       |********************                    |
       128 -> 255        : 46       |****************************************|
       256 -> 511        : 6        |*****                                   |
```