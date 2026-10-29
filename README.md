# ReelANSi

ReelANSi is a lightweight Linux viewer for ANSI and textmode art, built
for accurate rendering, smooth browsing, and classic BBS-style playback.

Point it at a file or a folder and enjoy the art.

ReelANSi is strictly a viewer, not an editor.

![ReelANSi](screenshots/reelansi.png)

## Download

**[Download ReelANSi v0.1 for Linux](https://github.com/Madp03t/ReelANSi/releases/tag/v0.1)**

Available as a portable AppImage for 64-bit Linux (x86_64). No Python or PySide6 installation required.

Download `ReelANSi-v0.1-x86_64.AppImage`, make it executable, and run it.

This is the current published release. Additional features described below are implemented in the development version and are planned for v0.2. Feedback and bug reports are welcome.

## Current Features

### ANSI Rendering

-   CP437 ANSI artwork
-   IBM VGA 9×16 font rendering
-   Classic 16-color VGA palette
-   Correct DOS/VGA foreground intensity handling
-   SAUCE-aware iCE color / high-intensity background rendering
-   SAUCE metadata, author/date, and artwork dimensions
-   Pixel-crisp rendering without text antialiasing
-   Viewport-aware painting for very tall artwork
-   Scroll artwork larger than the viewing area
-   Large ANSI loading/loaded indicator

### Files & Browsing

-   Open individual `.ANS`, `.ASC`, `.FLP`, `.ICE`, and `FILE_ID.DIZ` files
-   Open/select a folder containing supported textmode files
-   Automatically browse supported files in the same folder
-   `FILE_ID.DIZ` presented first when present
-   Previous / Next navigation with wraparound
-   Left/right arrow keyboard navigation
-   Clickable Previous / Next controls
-   Display the current filename and artwork dimensions
-   Display SAUCE author/date when available
-   Display the full folder path
-   Display the current file position within the folder
-   Reset artwork view to the top-left when changing files

### Animation & Playback

-   Progressive ANSI stream playback
-   Conservative automatic ansimation detection and playback
-   Play / Pause / Restart controls
-   Historical modem/BBS playback speeds from 300 baud through 230.4K
-   Instant playback for non-animated artwork
-   ANSI-encoded timing and padding respected during playback
-   Cursor movement, positioning, clearing, and screen overwrites during
    playback
-   Automatic viewport following during progressive playback, including
    tall ANSI files
-   Folder-wide autoplay, including progressive display of static artwork
-   Configurable pause between files during autoplay (5 seconds by default)
-   Autoplay stops at the end of the folder

### Export (development version)

-   Export complete static artwork as WebP or PNG
-   Export ansimations as animated WebP at the selected playback speed
-   Playback speed included in the suggested animated export filename
-   Native VGA-resolution export independent of viewport size and zoom
-   Export progress and cancellation for animated WebP

### Interface

-   F11 maximized / normal window toggle
-   Remembers normal window size and maximized state
-   Remembers playback speed
-   Horizontally centers artwork narrower than the viewport
-   Artwork zoom: 50%, 75%, 100%, 125%, 150%, and 200%
-   Fit artwork to window
-   Keyboard zoom controls: Ctrl++, Ctrl+-, and Ctrl+0
-   Current zoom percentage displayed in the interface
-   Minimal interface focused on the artwork

## In Development

-   Continued ANSI rendering fidelity testing against known-good scene
    artwork
-   Additional ANSI blink compatibility testing
-   XBin (`.XB`) support
-   Further ansimation compatibility testing, including tall animations

## Status

Early development. The published v0.1 AppImage remains available above.
The development version also includes folder autoplay and static/animated
WebP export, with PNG export for static artwork. These additions have been
tested locally and are not yet part of the published v0.1 AppImage.

## Development Approach

I have experience with programming, including professional and independent projects, but I'm not equally familiar with every language or technology. AI-assisted coding helps bridge those gaps and provides additional tools for developing and exploring solutions.

AI plays a significant role in writing and debugging code, particularly when working with technologies I'm less familiar with.

I determine the project's direction, design, and functionality, and handle testing and evaluation. While AI assists with implementation, the decisions about what gets built, what works, and what gets released remain mine.