# Mobile Implementation Resources - Global Area #

What is here:

* **full-site-link.vm** - This is how you build the link from the mobile version back to the desktop version of the site. The `$path` variable will dynamically generate the path that is used to build the link back to the desktop version. You will need to hardcode the output file extension and the desktop domain+leading folders as well.

* **mobile-detect-redirect.vm** - This is how you can detect a mobile device and automatically forward the user to the mobile version of that page. The `$path` variable will dynamically generate the path that is used to build the link. You will need to hardcode the output file extension and the mobile domain+leading folders as well.

* **outputs.vm** - This is how you can create links to different outputs of your page(s). The `$path` variable will dynamically generate the path that is used to build the links. You will need to hardcode the output file extensions and the desktop & mobile domains+leading folders as well.
