# doxygenBootstraped
Doxygen configuration which generates a web page with Bootstrap 4 components with online/offline import.

# Compatibility
### Important use Doxygen <= 1.8.11 !

# Directory Structure
.
├── Docs
├── Doxyfile
├── source
└── utils-bootstrap
    ├── RobotoSlab-Regular.woff2
    ├── RobotoSlab-Regular2.woff2
    ├── RobotoSlab-Regular3.woff2
    ├── RobotoSlab-Regular4.woff2
    ├── RobotoSlab-Regular5.woff2
    ├── RobotoSlab-Regular6.woff2
    ├── RobotoSlab-Regular7.woff2
    ├── bootstrap-doxy.css
    ├── bootstrap-doxy.js
    ├── customdoxygen.css
    ├── doxy-boot.js
    ├── footer.html
    ├── glyphicons-halflings-regular.eot
    ├── glyphicons-halflings-regular.svg
    ├── glyphicons-halflings-regular.ttf
    ├── glyphicons-halflings-regular.woff
    ├── glyphicons-halflings-regular.woff2
    ├── header.html
    ├── jquery-doxy.js
    ├── mainpage.md
    ├── roboto.css
    └── ~online_header.html

# Notes
All of the above files inside 'utils-bootstrap' are necessary to mantain the web page with Bootstrap without connection.
However, is preferable, if you know you will host it online, use the html file online_header instead of the default header (you can update Bootstrap easily changing the link for the css templates) by changing the name header -> ~header and online_header -> header (or setting it inside 'Doxyfile' file.

mainpage.md is a Markdown file which will be the home page of your generated web page. If you don't want to use it put '~' in front of it's name.

The folder 'Docs' will contain the generated web page (you can change it inside 'Doxyfile' file).
The folder 'source' will contain the source code where Doxygen pulls out their info (you can change it inside 'Doxyfile' file).


'doxy-boot.js' based in https://stratifylabs.co/embedded%20design%20tips/2014/01/07/Tips-Integrating-Doxygen-and-Bootstrap/
