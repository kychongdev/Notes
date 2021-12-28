px for borders and box shadows


em - based on nested div
rem - based on root
rem for font sizes

1. px for border widths, box shadows, etc.

2. em for font sizes

3. vw/vh is sometimes used for layout stuff

4. rem for margins and padding

5. ch I tend to use for things like paragraph text widths or sizing containers that will hold monospace fonts.


1. px for borders and box shadows: this stuff is for decoration. It's not generally required for readability. If a user sets a very large font size for themself, you don't necessarily want this stuff cluttering up the screen.

2. This is the only one where I'm sort of on the fence. It depends. If you're writing, modular, component-based CSS, then at the root of the component, I would be using a rem for sure. I don't want the font size of a parent component changing my sizes on one that's inside.

3. Yes. vw/vh for things that need to change with the size of the screen. A caveat for something that has width: 100vw; height: 100vh. The viewport units DON'T take scrollbars into account. So if you do the above and have a vertical scrollbar because of content overflow, you'll also get a horizontal scrollbar that scrolls the exact width of the vertical scrollbar. In this case, often width: 100%; height: 100vh; might work.

4. Yes. rem for paddings and margins. Unlike borders and box shadows, these DO affect the readability, and should grow with the font size.

5. Agreed. ch is a great unit. Studies have shown in the past that it's easiest for humans to read paragraphs that are between 50-70 letters across in width. So I often have a rule of something like p { width: 60ch; } or similar.