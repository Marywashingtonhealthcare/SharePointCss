# SharePointCss

Just a collection of CSS tricks and selectors that are used within SharePoint.  Will also include techniques and articles as appropriate.

To insert code into SharePoint pages, you have some options:

Option 1: Edit Source
Edit source will work in many cases, but if SharePoint doesn't like your code for some reason, it will strip out the markup. Beware of using this option.

Option 2: Embed Code or use Script Editor Web Part
When you use Embed Code, SharePoint actually creates a script editor web part for you and places it on the page. Slightly easier, but has marginal usability when your code starts to get more complex.

Option 3: Create a Document Library then refer to files within library with a CEWP (Content Editor Web Part)

Library can be called scripts or whatever you want. Best Practice is to use Site Assets, but doesn't really matter.

Individual scripts you can store as .html files. Txt files and .js files also work.

How to add to Content Editor:  Under Content Link, add the relative path to the file in your document library.

Option 3 is currently the preferred method. Why?
	• You can save the code centrally and then call it from multiple places without needing to replicate it
	• By saving it centrally, you only need to update it once if there are changes or updates
	• By saving it in the content database, you can access it from SharePoint Designer or similar, meaning you do not need to keep downloading-updating-uploading
	• It works consistently across all versions of SharePoint from SharePoint 2007 up to Office 365

What you can do:  You can make the file available across the site collection by placing the library in the root site and then you can make one change and have that change propagate out to every site in that site collection. Pretty cool...

