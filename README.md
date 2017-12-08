# Code Replacement Generator

*As a disclaimer, this code does nothing to bypass any security measures already set forth by CodeReplacement.com, it simply reinterprets any data that is already freely given to us by their interface.*

This code can be used to generate code replacements using the forms that are given for free on [CodeReplacement.com](http://codereplacement.com).

Many photographers use this website in tandem with software like [Photo Mechanic](http://www.camerabits.com/tour-v5/) to reduce workflow time in the editing process by using code to substitute intuitive variables with the names of players with their positions and team name. Similarly, we will be using code to scrape this data off the CodeReplacement.com website and generate our own copy-able text format.

The problem with that website is that the code replacement service comes with a fee and the form that is generated cannot easily be copy-pasted into a format that is easily understood by Photo Mechanic.

If you're tired of spending money for rosters or are just beginning to explore the usage of code replacements, this is a perfect tool to use in order to generate code replacements for free.

## Getting Started

### Prerequisites

To create your own free code replacements, all you need is a plain text editor. The built-in ones that come with many computers will suffice, Text Edit for Macs or Notepad for Windows. If you are using a Linux operating system, you could probably build this thing yourself.

Any browser that will let you save a page as HTML will work for this, but for the purposes of the tutorial, we will be using Google Chrome.

It is important to know that this process will work only for code replacement pages that generate a form for the user with each player's code, number, position and name. That being said, **this will not work for the NFL, NCAA Women's Basketball, Racing or Olympics** because the user will be prompted to `Download Roster File` instead of creating a form.

### Step-by-Step

1. Go to [CodeReplacement.com](http://codereplacement.com) like usual and create your custom prefixes and team names and click `Create Roster` at the bottom of the form when you're done.
2. A list should be generated with the names of all the players, their code, their number and their position. From here, (if on Chrome) right-click and select `View page source`.
3. Open two windows of your text editor, one empty and on the other, open the `cr-scraper.html` file.
4. Copy the entire contents of this file into your empty text editor.
5. In-between the `<html>` and `head` tags at the top of the file, insert a new, blank line. It should look like the following:
    ```
    <!DOCTYPE HTML>
    <html>

	    <head>
		    <title>...
    ```
6. Copy the entirety of the `cr-scraper.html` file and paste it at that blank line.
7. Save this as an HTML file, whatever you want to call it. On Notepad for Windows, you have to click the `Save as type` dropdown and select `All files` and then proceed to save it as `_________.html` in the file name.
8. Find this HTML file and open in in your browser.
9. You should now see at a button at the top of the page that says `Click for code`, click it.
10. Text should appear below that you can now copy and paste into a normal text editor that you can use as code replacements.

## Versioning

- V1.0: Works for most sports on the CodeReplacement.com page 

## Authors

* **Richard Dizon** ([GitHub](https://github.com/rcdizon), [LinkedIn](https://linkedin.com/in/rcdizon), [Photos](http://dizon.photos/)) - Please email `r.dizon@cavalierdaily.com` with any issues or suggestions to the code.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* [CodeReplacement.com](http://codereplacement.com) you provide a great service but sadly I'm just too cheap to justify buying that service from you all!
* StackOverflow, always been a great help.
* Anyone who is looking at this page right now, I'm open for freelancing! Check my portfolio [here](http://dizon.photos/).
