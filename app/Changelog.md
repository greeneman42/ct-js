## v 0.4.0

*13 September 2018*

### ⚡ General Improvements

* Add a room's name to its properties in the exported project
* Add a Shift modifier to place multiple copies or tiles at a room at once
* Add conversion to ES5
* Add QR codes and local addresses to the preview window
* Add tile culling
* Disable scaling and set proper width on mobile devices. Combine it with ct.fittoscreen to make your games mobile-ready (graphically)
* More consistent and intuitive tile and copy placement on grids in room editor
* More consistent behavior of ct.fittoscreen
* Move room templates to a JS object ct.rooms.templates
* Reorder room creation process to allow modifying room's view by copies' On Create code
* Set ct as a JavaScript object, move the canvas tag and all its properties to ct.HTMLCanvas

### ✨ New features

* Add `ct.touch` module
* Handling of copy-tile collisions with `ct.place.tile`
* Integrated debugger
* Show/hide certain tile layers

### 🍱 Demos

* Add a Platformer tutorial example project and its assets
* Update Catformer demo
* Update Catsteroids demo

### 🐛 Bugs Fixed

* Clean up logical assets after deleting a type or a graphical asset
* Fix checkboxes on the Settings tab not showing their saved state
* Fix HTML / CSS minification not working
* Fix preloader and random startup errors
* Room editor: Fix Shift and Ctrl modifiers working after a context menu was called.

### 💄 UI Improvements

* A bit better buttons
* Fix copy palette being visible on room's events screen
* Prevent clipping of sprite sheet settings at graphics editor on smaller screens. Move collision shape show/hide control to the left column.
* Tile editor improvements

### 📝 Docs

* Add a Platformer tutorial
* Add info about ct.js engine to docs' homepage
* Document ct.place.tile

### Other

* 📄 License: Remove edit prohibition for 3rd party libraries
* 💬 Rename 'Graphic' to 'Graphics'
* 🔖 Bump ct.fittoscreen version
* 🚚 🍱 Move SpaceShooter demo to a better location
* 🍱 Add a simple .desktop file for linux


## v0.3.1

*24 August 2018*

### ⚡ General Improvements

* Rectangular grids in room editor

### ✨ New Features

* Support for tilesets! **An early version, EXPERIMENTAL**

### 🐛 Bug Fixes

* Fix a bug preventing picking a background
* Fix a bug preventing to delete a room with a context menu
* Fix FPS input in graph editor not working
* Fix modal dialogues with 'Delete' labels instead of 'Ok'
* Replace JS minifier to support ES6

### 💄 UI Improvements

* Changes to number fields in style and graphic editors now affect preview panes instantly
* Search and sorting for room editor with minor UI improvements
* Show a warning when using duplicate names in assets

## v0.3.0

*17 August 2018*

### ⚡ General Improvements

- Add ct.draw.img as an alias to ct.draw.image
- Add optional x and y parameters to ct.draw()
- Git-friendly asset identifiers
- Make x and y in ct.types.copy optional
- Pre-initialize ct.types.list with empty arrays for each type
- Support new Keyboard API standard
- Update mouse position each frame
- Update mouse position each frame; better ct.mouse.imside resolution

### ✨ New Features

- 💄 Dark theme!
- Add a ct.sprite catmod

### 🐛 Bug Fixes

- Enable code checking in editors
- Fix an error in module.json of ct.canvas module
- Fix bugs when cancelling the an asset's duplicate creation
- Fix flipped orientation in ct.draw.imgext
- Fix pattern drawing with styles
- Fix pixelated render not fully working
- Fix styles' line width not exported correctly
- Fix texture selection in the styles editor
- Room size must be exported as numerical values
- Update the graphic asset in the editor's memory after replacing its source

### 💄 UI Improvements

- Add a "Copy the name" option to assets' context menus
- Better modal dialogues
- Custom Scrollbars
- Different minor UI improvements
- Open the sound after its creation
- Sort and search fields in resource views
- Wider room thumbnails

### 📄 License

Added license. TL;DR:

- You own your assets, projects, catmods;
- You can use the app for commercial use (and other uses too);
- You must not modify the ct.js in any ways that were not intended for it by the Author;
- We do not give any guarantees and are not responsible for any damage.

### 📝 Docs

- 🐛 Fix minor mistakes in ct.types docs

## v0.2.0

*05 August 2018*

### ✨ New features 

- 💄 More options for sounds and better UI
- Add custom scripts to your project
- Introduce ct.place.go and ct.place.trace methods
- Launch a static server for exported projects
- "Line — everything" collision detection in ct.place
- New ct.sound.howler module
- New ct.fittoscreen module

### ⚡️ General Improvements

- 🐛 Minor changes to the standart ct.sound
- 📝 Launch docs locally — now the docs for your particular version are bundled with ct.js and are available offline
- Make ct.mouse aware of possible view scrolling and scaling

### 🐛 Bug fixes

- Export unchecked ‘checkbox’ fields as false, not as an empty string
- Fix a bug in ct.draw.polygon.close, ct.draw.polygon.fill, ct.draw.polygon.stroke
- Fix ct.u.prect function not working with mirrored coordinates
- Fix exporter not copying includes folders of ctlibs
- Fix occasional failures while loading new images
- Fix wrong extensions of exported sounds

### 💄 UI improvements

- Make docs blue!
- Add a button to return to docs’ homepage
- Better presentation of ‘checkbox’ options of catmods
- Fix list overflow if there are too many resources

### 📝 Docs

- Add missing file extensions in “Creating your own mods” page
- Remove unexisting config fields of catmods, document the "help" field
- Reflect changes of ct.sound API

### 🍱 Updated demos

- Update Catformer demo with fullscreen option 
- Update Catsteroids with ct.sound.howler