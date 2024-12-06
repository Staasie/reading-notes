# Read 11

## Video and audio content

_Explain how the ability to use video and audio on the web has evolved since the early 2000s._

+ In the early 2000s, watching videos or listening to audio on the web relied on special software called "plugins," like Flash or QuickTime. You often had to download these plugins separately to make media work.

Today, you don’t need plugins anymore. Modern web browsers like Chrome, Firefox, and Safari can play video and audio directly using built-in tools, thanks to technologies like HTML5. This makes it faster, easier, and more secure to stream media on the web.

### **Example**

< video src="rabbit320.webm" controls >

  < p >

    Your browser doesn't support HTML video. Here is a
    <a href="rabbit320.webm">link to the video</a> instead.
  < /p >
</ video>

### **Example 2**

< audio controls >
  < source src="viper.mp3" type="audio/mp3" / >
  < source src="viper.ogg" type="audio/ogg" / >
  < p >
    Your browser doesn't support this audio file. Here is a
    < a href="viper.mp3" >link to the audio< /a> instead.
  < /p >
< /audio >

_Describe the use of the src and controls attributes in the < video > element._

+ In the same way as for the < img > element, the src (source) attribute contains a path to the video you want to embed. It works in exactly the same way.
+users have to be able to control the audio and video cause of things like epilepsy, at minimum it must include that.

_Why is it important to have fallback content inside the < video > element?_

+ Browser Compatibility: Not all browsers fully support the < video > element or specific video formats.
+ User Accessibility: Users on older devices or browsers may not be able to play videos.
+ Network Issues: If the video fails to load due to poor internet connectivity, fallback content provides a backup.
+ SEO and Accessibility: Fallback content can improve accessibility for screen readers and enhance search engine optimization.

_Write a very short story where < udio > and < video > are characters._

+ In the vibrant town of Webville, Audio and Video were siblings known for bringing stories to life.

Audio loved sharing songs and voices, filling the air with melodies and tales. Video, always the show-off, painted vivid pictures that danced and moved, captivating everyone who watched.

One day, an old visitor named Legacy Browser stumbled into town. “I’ve heard of your wonders, but I can’t keep up with your new tricks,” said Legacy.

Audio smiled warmly. “That’s okay. If you can’t hear my songs, I’ll leave behind a written note.”

Video nodded. “And if my movies don’t work, I’ll share a poster or a link.”

The visitor beamed. “Thank you! Now I can enjoy the magic in my own way.”

From then on, Audio and Video became Webville’s most inclusive entertainers, making sure no one missed the joy they brought.

## a complete guide to grid

_How does Grid layout differ from Flex?_

**Grid**
++ Best for creating two-dimensional layouts (rows and columns).
++ Useful when you need a structured layout like a webpage grid, photo gallery, or dashboard.
**Flex**
++ Best for one-dimensional layouts (row or column).
++ Useful for aligning items in a single direction, such as navigation bars or toolbars.

_Grid container, grid item, and grid line are a few important terms to understand when using Grid. Please describe these terms in a few sentences._

+ Grid Container: The parent element where the grid layout is applied using display: grid. It defines the grid structure and controls how child elements (grid items) are placed.

+ Grid Item: The direct children of the grid container. These are the elements that are arranged within the grid's rows and columns.

+ Grid Line: The horizontal and vertical lines that divide the grid into rows and columns grid items can be placed and sized relative to these lines.

## Responsive images

_Besides making a site visually appealing across different screen sizes, why should developers make images responsive?_

+ improved performance, better accessibility, SEO benefits and device compatibility.

_Define the following < img > attributes srcset and sizes. Write an example of how they are used._

### **srcset**

+ Specifies a list of image file URLs with different resolutions or sizes.Allows the browser to choose the most appropriate image to load based on the device's resolution or viewport size.

### **sizes**

+ Defines the layout width (in CSS units) that the image will occupy in different scenarios.
+ Helps the browser decide which image from the srcset to download.

**Exapmle**
<img
  src=

  small.
  
  jpg"

  srcset="
    small.jpg 480w,
    medium.jpg 800w,
    large.jpg 1200w"
  sizes="(max-width: 600px) 100vw, (max-width: 1200px) 50vw, 33vw"
  alt="A beautiful landscape">

_How is srcset more helpful for responsive images than CSS or JavaScript?_

### **Browser Optimization**

 The browser automatically selects the most appropriate image from the srcset based on the device's resolution and screen size.
No additional calculations or scripts are needed, reducing overhead.
Reduced Latency:

+ The decision is made before the image is downloaded, ensuring only the best-fit image is loaded. CSS and JavaScript often require extra steps to manipulate or resize images after they’re already loaded.
Built-in Responsiveness:

+ With srcset, you don’t need additional CSS media queries or JavaScript logic to handle varying screen sizes. The browser handles responsiveness natively.
Bandwidth Efficiency:

+ Users on devices with smaller screens or slower connections are served smaller images, conserving bandwidth and improving loading speed.
Simpler Code:

+ With srcset, you define everything within the < img > tag, avoiding complex CSS or JavaScript logic.
Accessibility and SEO:

+ Browsers fully understand the < img > element with srcset, maintaining proper semantics for search engines and screen readers.

### **why does css an JavaScript fall short**

+ CSS: Can only control the display size of an image, not the actual file that is downloaded.
A large image will still be downloaded even if displayed at a smaller size, wasting bandwidth.

+ JavaScript: Requires additional scripting and may add complexity and execution delays.
Not as fast or efficient as the browser's native decision-making.
