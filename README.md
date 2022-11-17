# IEDC Blog

## Setup

Install Hugo by following instructions [here](https://gohugo.io/getting-started/installing/)

Then clone this repo using:

```sh
git clone https://github.com/IEDCMEC/iedc-blog.git
```

or with ssh

```sh
git clone git@github.com:IEDCMEC/iedc-blog.git
```

#### Starting dev server

```sh
hugo server -D
```

#### Adding CSS or JS

Create the css file in assets/css/<filename>.css

For JS create the file as assets/js/<filename>.js

Edit the following entries in the file config/\_default/params.toml as

```toml
customCss = ["css/file1.css", "css/file2.css" ]
customJs = [ "js/file1.js", "js/file2.js" ]
```

## Adding images in post

- Create a folder corresponding to the post in static/images
- Paste the image in this folder
- Referrence this image in <post>.md using markdown syntax with path as `/images/<folderName>/imageName.jpg`
- (check markdown file of any other blog post with image for example)

## For adding profile image

- Paste the author image in static/authorImages
- Write the image file name with extension in the front matter of the post under the "image" property.
  - eg: `image: "johndoe.jpg"`
