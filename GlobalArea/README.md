# Mobile Implementation Resources - Global Area #

What is here:

* **full-site-link.vm** - This is how you build the link from the mobile version back to the desktop version of the site while also providing a PHP query string for capturing the redirect. The `$path` variable will dynamically generate the path that is used to build the link back to the desktop version. Wrapping the path in the `system-asset` tags that also make sure of the `:configuration` pseudo-class, Cascade will track/manage the link and make sure the full URL is written during the publish process (domain pulled from the Destination and output file extension pulled from the corresponding Configuration Set).

* **mobile-detect-redirect.vm** - This is how you can detect a mobile device and automatically forward the user to the mobile version of that page. The `$path` variable will dynamically generate the path that is used to build the link. You will need to hardcode the output file extension and the mobile domain+leading folders as well. This script also has the ability to capture the presence of a query string for stopping the redirection after the user has explicitly chosen to go back to the desktop version.

* **outputs.vm** - This is how you can create links to different outputs of your page(s). The `$path` variable will dynamically generate the path that is used to build the links. You will need to hardcode the output file extensions and the desktop & mobile domains+leading folders as well.
