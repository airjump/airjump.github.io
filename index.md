## Welcome to my Project - Page

### Preamble

I will try to document everything here in English. The goal is to share my knowledge with many in the community. The project should be an attempt to illuminate the aspect of security and to gain experience around the topic of networks and Linux. The best way to contact me is about Twitter: [@airjump](https://twitter.com/airjump)

### Insertion and Testing

Admittedly, I got some very nice hints and three new tools that help me to describe and document the project better. [@sl0](https://twitter.com/JohaPrime) Thanks.

1. [ditaa](http://ditaa.sourceforge.net/)
2. [nwdiag](http://blockdiag.com/en/nwdiag/index.html)
3. [aafigure](https://pythonhosted.org/aafigure/)

I put the test with the tools to the Git. [GIT](https://github.com/airjump/scripte.git)

#### First Results

```markdown
nwdiag {
  Internet [shape = cloud];
  Internet -- router;

  network {
    router;
    Raspberry PI;
  }
}
```

![First](https://github.com/airjump/scripte/blob/master/first.png?raw=true)

### Project - Description

A picture says more than a thousand words. Nevertheless, a few sentences about the project. The goal is to set up a "filter" with a Raspberry PI and two USB network cards. The two network cards should not become logically visible. On the Raspberry PI runs a Linux which is configured (I hope).

#### Visualization

![Finished](https://raw.githubusercontent.com/airjump/scripte/master/doc-network.png)

### Preparations
The order of the USB network cards is out. Delivery has been made. The Raspberry PI has been ordered and delivered.
The next step is a checklist with all materials to unpack or unboxing :-) .


| No  | Description  | Count  | Link  |
|---|---|---|---|
| 01  | Raspberry Pi 3 Model B+  | 1  | https://www.raspberrypi.org/products/raspberry-pi-3-model-b-plus/  |
| 02  |  USB 3.0 auf RJ45 Gigabit Ethernet  | 2  | https://www.anker.com/de/products/variant/aluminum-usb-3-0-auf-rj45-gigabit-ethernet-adapter/A7611011  |
| 03  | SD Card  | 1  | https://www.sandisk.com/home/memory-cards  |
| 04  | Network Patch Cables  | 3  | -  |
| 05  | RASPBIAN STRETCH WITH DESKTOP  | 1  | https://www.raspberrypi.org/downloads/raspbian/  |
| 06  | PC  | 1  | -  |
|   |   |   |   |

------------------------------------------------------------------------

## Testing

Not quite finished but it comes. :-) 

```markdown
nwdiag {
  Internet [shape = cloud];
  Internet -- router;

  network ISP {
      router;
      Raspberry-PI;
  }
  network internal {
      Raspberry-PI;
      Host_01;
      Host_02;
  }
}
```

![Schematic Representation](https://github.com/airjump/scripte/blob/master/schematic_representation.png?raw=true)

#### Experimental


```markdown

 Internet service provider (ISP)

            +
            | xDSL Interface
            |                              Raspberry PI               +-----+
            |                                                         |     | ETH1-N
          +-+-----+                           +----+                  |     +----------+ PC/ PAD/ ...
          |       +---------------------------+    +------------------+     |
          |       | ETH0             USB ETH1 |    | USB ETH2         |     +----------+ PC/ PAD/ ...
          +-------+                           +-+--+                  +-----+
                                                | ETH0
 Home Router (RD) or Home Gateway (HG)          |                     Switch
                                                |
                                                |
                                                | ETH0
                                           +----+----+
                                           |         |
                                           |         |
                                           +---------+

                                            UBUNTU PC

```

![Picture 1](https://farm5.staticflickr.com/4882/31878653118_7b9627fd9e_b.jpg)
