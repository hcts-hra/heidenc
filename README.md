# heidENC

Bibliography of Chinese Encyclopaedic Works 1840-1937, their Japanese and Western Models and Sources.

<!-- TODO(DP): Link heiData see #6 -->

This repo contains the contents of the last archived word document converted to markdown to deploy a statically hosted webpage.

The original project has been split into three parts:

- This Repo.
- A [data repo](https://github.com/hcts-hra/heidenc-txt) for professionally typed `.txt`  files of primary sources (incomplete)
- a [Data publication](https://zenodo.org/record/7313202) for binary files

## Development

Corrections and contributions to the bibliography are welcome:

1. Follow the instructions below to start a local copy of the webpage.
2. Edit contents
3. Open a pull request

## Requirements

- [Hugo](https://gohugo.io)

To install Hugo please follow the steps outlined in [their documentation](https://gohugo.io/getting-started/installing/) for your platform.  

## Local Installation

Before you can get a copy of the webpage up and running locally on your machine, you need to clone this repo. The [blowfish theme](https://github.com/nunocoracao/blowfish/) is installed as a submodule.

```bash
git clone --recurse-submodules --remote-submodules https://github.com/hcts-hra/heidenc.git
```

If you forgot to include the submodule flags when cloning the repo run the following:

```bash
git submodule update --init
```

To just update the theme.

```bash
git submodule update --remote --merge
```

## Building

To build a local dev version run:

```bash
hugo server -D  
```

You should see something like this:

```bash

                   | EN   
-------------------+------
  Pages            |  57  
  Paginator pages  |   0  
  Non-page files   |   0  
  Static files     | 218  
  Processed images |   0  
  Aliases          |  11  
  Sitemaps         |   1  
  Cleaned          |   0  

Built in 150 ms
Watching for changes in ~/Documents/GitHub/heidenc/{archetypes,content,static,themes}
Watching for config changes in ~/Documents/GitHub/heidenc/config.toml
Environment: "development"
Serving pages from memory
Running in Fast Render Mode. For full rebuilds on change: hugo server --disableFastRender
Web Server is available at http://localhost:1313/ (bind address 127.0.0.1)
Press Ctrl+C to stop
```

Congratulations, the page is visible in your browser at [http://localhost:1313/](http://localhost:1313/)
