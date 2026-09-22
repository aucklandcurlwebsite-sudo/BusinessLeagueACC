# Club Website Template

## Included

The complete public website and Admin dashboard are contained in index.html.
The package preserves the photo fan, live preview, image placement,
round robin, announcements, hyperlink controls and named CSS interactions.

## Design and Zones

Club colours:
- Merino: #F5EEDD
- Rock Blue: #84B3CE
- Venice Blue: #16587B

Website zones:
1. Header and navigation
2. Hero
3. Announcements
4. About the club
5. Round Robin
6. Photo gallery
7. News and posts

## Website Editor

Admin provides club-name and colour controls, hero text and button editing,
about text editing, and gallery heading editing.
The live preview renders a scaled copy of the public page.

## Announcements

Edit announcement text, background and text colours, alignment, size,
vertical spacing, letter spacing, bold and uppercase styling, visibility,
destination link and new-tab preference. Save Changes confirms saving.
Use club colours restores the announcement's colour connection to the theme.

## Photo Library and Gallery

Photo Library stores uploaded images for selection and placement.
Drag a library thumbnail onto the preview's hero, about image or photo fan.
The Image Placement controls provide a button alternative to dragging.

Photo Fan Gallery uploads go directly into the gallery.
The fan displays the latest five photos; clicking opens a viewer that can
browse all gallery images. Previous, next and keyboard controls are included.
Gallery thumbnails let you choose a photo for image adjustments.

Images are resized and compressed for browser storage. Upload and storage
errors are displayed. There is no fixed eight-photo limit, but browser
storage capacity still applies.

## Image Placement

Select hero, about image or photo fan, then adjust horizontal position,
vertical position and zoom. Save Changes confirms the adjustments.
Zoom is calculated from the image's fitted size.

## Round Robin

- Add and rename teams.
- Generate a schedule in which every team plays each opponent once.
- Give byes when the roster has an odd number of teams.
- Enter, edit or clear match scores.
- Calculate played, wins, draws, losses, score difference and points.
- Award 3 points for a win, 1 for a draw and 0 for a loss.
- Display results and standings on the public page.

Adding and removing teams is locked after fixture generation.
Reset fixtures clears fixtures and scores after confirmation, allowing
roster changes. Team names remain editable.

## Hyperlinks

Hyperlinks appears directly below Interactive Hyperlinks in Admin.

Link Location selects a website zone. Link text searches existing words
in that zone, ignoring case. It links existing text rather than adding
new words. A missing match produces a message.

Link to selects a named destination zone, or use a custom web, email,
telephone or section address. Choose a hover effect and new-tab preference,
then Save Changes. Existing links can be edited or removed.

The current search uses the first matching text node; phrases spanning
separate HTML elements may not match. Existing anchors are updated as a
whole when matched.

## Named Interactive Effects

Interactive Hyperlinks includes:
- Link text and destination
- Hover interaction dropdown
- Live Interaction Preview
- Saved custom interaction selector
- New interaction button
- Interaction name
- Custom hyperlink CSS textbox
- Save Code button
- Apply Effect to Website button

Save Code stores each named effect separately and selects it for preview.
Saved effects appear by name in both hover dropdowns.
Renaming an effect retains its identity for links already using it.

Apply Effect to Website uses the entered link text and destination to
update matching existing website links with the selected effect.
Use Hyperlinks first if the desired text is not yet a link.

Custom CSS supports .interactive-link and standalone button/link selectors,
including .btn and .liquid. Supported rules are scoped to the selected
effect. Demo body styling is excluded from the website.
This field is for CSS, not arbitrary HTML or JavaScript. Complex selectors,
extra HTML structures and some CSS rule types may require adaptation.

Example liquid effect:

```css
.btn {
  position: relative;
  padding: 1rem 2rem;
  font-size: 1rem;
  font-weight: 600;
  color: white;
  background: none;
  border: 2px solid #646cff;
  border-radius: 8px;
  cursor: pointer;
  overflow: hidden;
  transition: all 0.3s ease;
}
.liquid {
  background: linear-gradient(#646cff 0 0) no-repeat
    calc(200% - var(--p, 0%)) 100% / 200% var(--p, 0.2em);
  transition: 0.3s var(--t, 0s),
    background-position 0.3s calc(0.3s - var(--t, 0s));
}
.liquid:hover {
  --p: 100%;
  --t: 0.3s;
  color: #fff;
}
```

## Storage and Limitations

This package contains the source template and default content.
It does not include user edits, uploaded images, custom effects or results
held in an existing browser's storage.

Website content uses browser storage key clubWebsiteLiveEditorV1.
Round robin data uses club-round-robin-v1.
Data is local to the browser and is not shared across devices.
File moves, renames or browser-data clearing can affect access to saved data.

A password prompt now appears whenever Admin is opened. Closing the dashboard
requires entering the password again on the next opening. The source stores
a password digest rather than the plaintext password.
This browser-side lock can be bypassed by someone who controls the file or
browser; there is no secure server-side authentication, hosted database or
deployment in this package.
News posts are currently template content rather than a full post editor.
Sample photos require internet access.

## Verification

Prior focused checks covered scheduling for 2-32 teams, scoring,
photo-saving logic, named-effect persistence and CSS selector conversion.
Scripts have been checked for JavaScript syntax.
Full visual browser verification remains incomplete because local browser
testing was blocked in the working environment.

## Future Changes

Use this latest file as the base. Preserve existing features when adding
or fixing functionality; do not replace it with the older website prototype.
