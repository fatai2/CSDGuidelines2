# CSD Guidelines
![Expo Publishing](https://github.com/fatai2/CSDGuidelines2/workflows/Expo%20Publishing/badge.svg)
 
# CSD Guidelines

The CSD Guidelines app is designed to provide offline access to the updated guidelines of the Clinical Services Department of the MRCG. It does this by providing over-the-air updates whenever any change in this repository is committed. This minimizes the number of new builds of apps that need to be released.

# Usage

  - Upload a properly formatted CSD Guideline in WORD (docx. only) into the "docs" folder and watch it magically convert into an HTML file stored in the "www" folder
    -- Pictures in the Word document should be saved as PNG format and re-inserted into the docx. file before uploading. This will prevent the converter from using the default EMF format that will NOT display in the app.
    -- Simplify tables
    -- Simplify complex charts and diagrams: This can be done by grouping components of each diagram into single objects, saving them as PNG files, delete the diagram and insert the picture file to replace it in the document.
    -- File names should be in the standard CSD Guidelines format
  - Changes to be highlighted in the "What's New" section of the app can be saved in text files in the "changes" folder under "www". Each new file should contain the date and the contents of the change.  Save with incrementing numbers e.g "1.txt", "2.txt"
  - Commit changes to "master"
  - - Congratulations! Changes made will now reflect on users' apps!

### Tech

The CSD Guidelines incorporates/ is a modification of a number of open source projects:

* [Expo] - For over-the-air updates and building iOS, Android and Web Apps!
* [React Native] - Javascript codes for mobile deployment
* [Github Actions] - For continuous deployment and continuous integration
* [twitterClone] - Design and code for app
* [Pandoc] - conversion of document formats
* [GitHub Pandoc HTML5 Template] - Sleek template for HTML5 output files in [Pandoc]

### Building apps

The Android app for this version is already built and deployed. To build a new version of the app or an iOS version, replace the final expo publish line in the [.github/workflow/expo-publish.yml] file with the appropriate expo command 



[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen. Thanks SO - http://stackoverflow.com/questions/4823468/store-comments-in-markdown-syntax)


   [twitterClone]: <https://github.com/Trancever/twitterClone>
   [pandoc]: <https://pandoc.org/index.html>
   [Expo]: <https://expo.io/>
   [React Native]: <https://reactnative.dev/>
   [Github Actions]: <https://github.com/actions>
   [GitHub Pandoc HTML5 Template]: <https://github.com/tajmone/pandoc-goodies/tree/master/templates/html5/github>
