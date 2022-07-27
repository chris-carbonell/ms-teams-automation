# Overview

send <b>GIFs</b> in <b>MS Teams</b> using <b>PyAutoGUI</b>

# Why?

Some environments do not permit users to have access to the Microsoft Graph API behind MS teams. 

Despite those restrictions, we can still have fun by using PyAutoGUI to spam our loved ones with funny GIFs.

# Quickstart

I recommend just using the Jupyter notebook to run the code so you can update the Giphy search terms and other parameters on the fly.

The <code>send_gifs.ipynb</code> notebook contains a couple of functions depending on your needs:<br>
* <b>send_gif</b><br>
send one GIF for a given search term
* <b>send_multiple_gifs</b><br>
send multiple GIFs for a given search term
* <b>send_mulitple_terms</b><br>
send multiple GIFs for multiple search terms

# Installation

Install the required dependencies with the following:<br>
<code>python -m pip install -r requirements.txt</code>

# Notes

* The <code>GIF_LOCATIONS</code> constant specifies the <b>relative</b> locations of the GIFs relative to the GIF button. Your environment might have those locations in slightly different positions so you'd have to update those locations as necessary.
* Loading the first GIF can be slower depending on which search terms have been cached recently. Therefore, I add some lag for the first load of a given search term.

# Resources

* Tutorial<br>
https://ayushi7rawat.medium.com/how-to-automate-ms-teams-with-python-6a5ca1b62cb2
* Repo<br>
https://github.com/ayushi7rawat/MS-Teams-Automation/blob/master/script.py