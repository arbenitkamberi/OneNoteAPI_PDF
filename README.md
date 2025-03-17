Creates a new page in OneNote containing the PDF you uploaded in high resolution.
Deployed using [GitHub Pages](https://arbenitkamberi.github.io/OneNoteAPI_PDF/)

# Why? 
OneNote on Mac used to have awful resolution when inserting a PDF, so I made this & used it extensively during my studies as I was already on OneNote before buying a Mac & didn't want to switch.

# How does it work?
It uses PDF.js to render the each page of the PDF in the browser, then uploads that page as an image to your notebook using OneNotes GraphExplorer API.
It also extracts URLs present in each page to add those links in your notebook as well, which OneNote still doesn't do :).

# How to use
Clicking on the "Authentication Token"-link opens a tab where you can log-in to your microsoft-account, then press on "Access token" to copy and paste it into the text-input. The authentication token will be saved locally, so you only need to do this once in a while.
Select the notebook you're working on, then the section. Give the new notebook-page a name and upload the pdf. Using the slider you can change the size of the render (thus the resolution that the pdf will be uploaded in), it will show you a preview from the first page of the PDF. Press create.

## Setting Favorite Notebooks
If you have lots of notebooks like me, you can set a localStorageitem to display those and collapse the rest of the notebooks.
Ex:

  `localStorage.setItem("notebookFavs", '["Intro to Machine Learning", "Information Security", "Compiler Design", "Computer Systems"]');`

There's no UI for that as I changed my favs only once every semester.
