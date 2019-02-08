# Suppliers in Novosibirsk

This repository contains template for suppliers website. It uses [jinja2](http://jinja.pocoo.org/) templates. And might be compiled with [staticjinja](https://staticjinja.readthedocs.io/).

To install all the requirements use next line:
```
pip3 install -r requirements.txt
```

Project has next structure:

```
.
├── README.md
├── public                      # result files
│   ├── assets                  # public assets
│   ├── index.html
│   └── requests.html
├── requirements.txt
├── sketches                    # original mockups
└── templates                   # directory with templates
    ├── components              # jinja2 components/partials
    │   ├── common              # common components (across the pages)
    │   └── main                # page specific components

    ├── index.html
    └── requests.html
```

### For development:

```
staticjinja watch --srcpath=templates --outpath=public
```

Using 
```
livereload public/
```
also might be usefull

### To build:

```
staticjinja build --srcpath=templates --outpath=public
```


# Project Goals

The code is written for educational purposes. Training course for web-developers - [DEVMAN.org](https://devman.org)
