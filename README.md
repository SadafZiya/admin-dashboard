# admin-dashboard

An admin dashboard layout in plain HTML and CSS: a sidebar of navigation items, a topbar, cards of
figures, a recent-orders table and a customer list.

No framework and no build step — open `index.html`.

## The two moving parts

`assets/javascript/main.js` does only two things:

- The sidebar item under the cursor gets a `hovered` class, which is what draws the curved cut-out
  joining the item to the panel edge. The class is removed from every other item first, so only one
  is ever curved.
- The menu button toggles `active` on both the sidebar and the main area, collapsing the sidebar to
  icons and letting the content spread into the space.

Everything else — the layout, the card grid, the table, the responsive breakpoints — is CSS.

## The notebook

`change-image-color.ipynb` is a one-off utility used to recolour the icon set, not part of the
page. It is excluded from GitHub's language stats in `.gitattributes`, since by byte count it
would otherwise outweigh the HTML and CSS and label the whole repository as a notebook.
