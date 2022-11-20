My userChrome.css file

#Installation

First, find your user profile folder. It can be found at: Hamburger menu > Help > More troubleshooting information, and clicking "open folder" under "Profile directory"

To install userChrome, input the following command in your terminal while CD'd into your current user profile folder:

	git clone git@github.com:kagent42/userChrome.git && mv userChrome chrome

If you don't have an SSH connection with Github, you can use HTTPS instead:
	
	git clone https://github.com/kagent42/userChrome.git && mv userChrome chrome

After this step, the following changes should be made in Firefox's about:config page:

-> set `toolkit.legacyUserProfileCustomizations.stylesheets` to `true`

Then everything should be working

