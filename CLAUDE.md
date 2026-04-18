# Project Description / Initial Prompt
This is a small URL calculator / login step by step guide for using a claude
ai oauth URL with codespaces. It is coded completely in vanilla javscript within
a single file, index.html.

When the user opens the page, they will see the curl installation instructions
for installing claude code. This will be in a box for easy copying, and displayed
as shell code. There will also be a box for them to paste the claude auth URL
which will allow the user to paste the URL. The javascript application should 
then extract the port number from the redirect_url field of the oauth URL. 
The redirect URL will look like this: localhost:portnumber/callback. The user 
will then be prompted for this information:

"Paste the codespace port forwarding URL for port <portnumber>"

Allow the user to paste this URL. The prompt should take the form of this 
text and entry box appearing on the screen. Not a dialog box. This is a step
by step process that guides the user through creating the authorization they required.

Once we have the port forwarding URL, display a hyper link to the original
authorization URL, prompting the user to click there and authorize claude code.
This should open in another window/tab, keeping this page as it is.

Now, prompt the user for the URL that failed. This will be of the form of 
the rediruect URL. The application will then generate a URL that looks like this:

<codsepace port forward URL>/callback/...

Where "callback" to the end is from the pasted URL.

Provide a user with a link to this newly formed URL which will also open in a
new window.

Tell the user that if they saw "build something great" then they are done.

# Attribution
Be sure to list yourself as the coauthor of any commit and push you make.
List yourself in such a way that it sites the https://github.com/claude account
/ org.

# Logging
After each major step / commit, summarize the development effort that led
there and append it to "DEVLOG.md". Just append to this file, do not read it.
Keep the summaries short, about 3-5 lines for the summary, though give some
indication of what was prompt and what was response.

Always include DEVLOG.md in every commit, staging it alongside any other
changed files.