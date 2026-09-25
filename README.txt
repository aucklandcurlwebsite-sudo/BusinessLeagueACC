CLUB WEBSITE TEMPLATE
Packaged 22 September 2026

GET STARTED
1. Extract the ZIP folder.
2. Open index.html in a modern browser.
3. Click Admin and enter your configured password to edit the website.

FILES
index.html - Complete website, Admin dashboard, CSS and JavaScript.
PROJECT-NOTES.md - Features, workflow and known limitations.
SLIDE-CONTENT-NOTES.md - Content imported from slides 4-7 of the supplied deck.
assets/auckland-curlers.jpg - Curling team photograph from slide 6.

Keep the assets folder beside index.html so the imported photograph loads.

No installation or local server is required.
The sample gallery photos load from the internet.

SAVED CONTENT
Admin has one Undo button in its top bar instead of Default/Reset controls.
It restores the previous change, including round-robin data, and saves it.
Repeated clicks step backwards through recent changes in this open session.
Undo history is kept in memory and clears when the page is reloaded.

The Blog flip book editor supports a book title, visibility, cover photos,
post titles, authors, dates and post text. Publish post places a new post
at the front. Editing a published post keeps its position. Save draft keeps
the current editing draft without publishing it. New post replaces that draft.
The book starts closed. Click the cover or the right arrow to open it.
Readers can turn pages by dragging a page edge, using the arrow buttons,
or pressing left/right arrow keys. The return-to-cover button closes the book.
On narrow screens the book shows one page at a time. Long text can scroll
inside its page without turning the page. New posts remain at the front.
The included StPageFlip 2.0.7 library works offline and is MIT licensed;
see assets/page-flip-LICENSE.txt. Its render loop has a local cleanup fix
to release old book instances when posts are changed in the editor.
Blog posts and drafts are stored in this browser, like other Admin edits.

Admin edits and uploaded photos are stored in your browser, not written
back into index.html. This package includes the template code and default
content. It does not export photos, scores or edits stored in your browser.
Opening this copy at a new file location may start with default content.
Keep your existing website file and browser data to retain existing edits.

This is a local prototype with a browser-side password prompt. It does not provide secure server-side Admin authentication,
online publishing or shared storage across devices.
