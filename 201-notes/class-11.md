## Class 11 Reading Notes


#### Video and Audio Content

1.Explain how the ability to use video and audio on the web has evolved since the early 2000s.
  
  Prior to the introduction of `video` and `audio` techologies like flash and silverlight were used to incorperate video and audio to websites. These older methods usually had security and acessiblity issues, these were later phased out due to HTML elements like `video` and `audio`. These elements can be controled by JavaScript API's



2.Describe the use of the src and controls attributes in the `<video>` element.

  **src** works the exact same way it works for `<img>` element. the `src` attribute contains a path tot he video that you want to embed.


3.Why is it important to have fallback content inside the `<video>` element?

  Fallback content is conten that will be displayed if the browser accessing the page doesn't support the `<video>` elemement, allowing us to provide a fallback for older browers. This can be anything. The goal is to provide the user a method of viewing the content no matter the browser they are using. 


4.Write a very short story where `<audio>` and `<video>` are characters.

  Audio and video are super heroes in a galaxy far away. They work together to make content accessible accross the universe. 

#### A Complete Guide to Grid

1.How does Grid layout differ from Flex?

One of the ways that Grid layout differes from Flex is that it is 2 dimensional compared to 1. 


2.Grid container, grid item, and grid line are a few important terms to understand when using Grid. Please describe these terms in a few sentences.

Grid container is the direct parent of other grid elements, grid item are the children/decendants of the grid container.



#### Responsive Images  

1.Besides making a site visually appealing across different screen sizes, why should developers make images responsive?

Resoponsive images also lead to faster load times for mobile devices as they load quicker compared to non responsive images.

2.Define the following `<img>` attributes srcset and sizes. Write an example of how they are used. 

`srcset` attribute defines the set of images you allow the browser to choose between. 

For each image we write: 

1. An image filename (elva-fairy-480w.jpg)
2. A space
3. The image's intrinsic width in pixels (480w) — note that this uses the w unit, not px as you might expect. An image's intrinsic size is its real size, which can be found by inspecting the image file on your computer (for example, on a Mac you can select the image in Finder and press Cmd + I to bring up the info screen).


>
    <img
    srcset="elva-fairy-480w.jpg 480w, elva-fairy-800w.jpg 800w"
    sizes="(max-width: 600px) 480px,
         800px"
    src="elva-fairy-800w.jpg"
    alt="Elva dressed as a fairy" />


>

`sizes` defines a set of media conditions and indicates what image size would be best to choose, when certain media conditions are true

3.How is srcset more helpful for responsive images than CSS or JavaScript?

1. A media condition ((max-width:600px)) — you'll learn more about these in the CSS topic, but
for now let's just say that a media condition describes a possible state that the screen can
 be in. In this case, we are saying "when the viewport width is 600 pixels or less".

2. A space

3. The width of the slot the image will fill when the media condition is true (480px)



#### Things I want to know more aboout

  Using an API to interact with audio and visuals.


#### References 

[Repsponsive Images](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images)