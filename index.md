## Welcome to my Project - Page

### Preamble

I will try to document everything here in English. The goal is to share my knowledge with many in the community. The project should be an attempt to illuminate the aspect of security and to gain experience around the topic of networks and Linux. The best way to contact me is about Twitter: [@airjump](https://twitter.com/airjump)

### Project - Description

A picture says more than a thousand words. Nevertheless, a few sentences about the project. The goal is to set up a "filter" with a Raspberry PI and two USB network cards. The two network cards should not become logically visible. On the Raspberry PI runs a Linux which is configured (I hope).

#### Visualization

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

------------------------------------------------------

You can use the [editor on GitHub](https://github.com/airjump/airjump.github.io/edit/master/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/airjump/airjump.github.io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.

![Image of Yaktocat](https://octodex.github.com/images/yaktocat.png)
