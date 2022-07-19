# IEDC Blog

## Setup
Install Hugo by following instructions [here](https://gohugo.io/getting-started/installing/)

Then clone this repo along with the submodules
```sh
git clone https://github.com/IEDCMEC/iedc-blog.git --recursive
```
or with ssh
```sh
git clone git@github.com:IEDCMEC/iedc-blog.git --recursive
```

#### Starting dev server
```sh
hugo server -D
```

#### Adding CSS or JS
Create the css file in assets/css/<filename>.css

For JS create the file as assets/js/<filename>.js

Edit the following entries in the file config/_default/params.toml as
```toml
customCss = ["css/file1.css", "css/file2.css" ]
customJs = [ "js/file1.js", "js/file2.js" ]
```
