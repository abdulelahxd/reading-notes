# images 
Images should 
1. Be relevant
2. Convey information
3. Convey the right mood
4. Be instantly recognisable
5. Fit the color palette

>If we are building a site from scratch, it is good practice to create a folder for all of the images the site uses. 
>As a website grows, keeping images in a separate folder helps you understand how the site is organized. Here you can see an example of the files >for a website; all of the images are stored in a folder called images.
>On a big site you might like to add subfolders inside the images folder. For example, images such as logos and buttons might sit in a folder called >interface, product photographs might sit in a page called products, and images related to news might live in a folder called news.


To add an image into the page you need to use an``` <img>``` element. This is an empty element (which means there is no closing tag). It must carry the following two attributes: 

1. **src** This tells the browser where it can find the image file. This will usually be a relative URL pointing to an image on your own site. (Here you can see that the images are in a child folder called images — relative URLs

2. **alt** This provides a text description of the image which describes the image if you cannot see it.

3. **title** You can also use the title attribute with the ```<img>``` element to provide additional information about the image. Most browsers
will display the content of this attribute in a tootip when the user hovers over the image.

4. **height** This specifies the height of the image in pixels.

5. **width** This specifies the width of the image in pixels. Images often take longer to load than the HTML code that makes up the rest of the page.
It is, therefore, a good idea to specify the size of the image so that the browser can render the rest of the text on the page while leaving the right amount of space for the image that is still loading.



## Three Rules for Creating Images
There are three rules to remember when you are creating images for your website which are summarized below. We go into greater detail on each topic over the next nine pages

1. Save images in the right format
2. Save images at the right size
3. Use the correct resolution


JPGs, GIFs, and PNGs belong to a type of image format known as bitmap. They are made up of lots of miniature squares. The resolution of an image is the number of squares that fit within a 1 inch x 1 inch square area.

Images appearing on computer screens are made of tiny squares called pixels. A small segment of this photograph has been magnified to show how it is
made up of pixels. The web browsers on most desktop.

computers display images at a resolution of 72 pixels per inch (ppi). Images in print materials (such as books and magazines) are made up of tiny circles called dots. These images are usually printed at a resolution of 300 dots per inch (dpi).

![VvsB](https://www.presentationteam.com/wp-content/themes/yootheme/cache/StickerYou_Blog_Vector-vs-Bitmap_600x400-13e51a05.jpeg)

Vector images differ from bitmap images and are resolution-independent. Vector images are commonly created in programs such as Adobe Illustrator.

Animated GIFs show several frames of an image in sequence and therefore can be used to create simple animations.

```<figure>``` Images often come with captions. HTML5 has introduced a new ```<figure>``` element to contain images and their caption so that the two are associated. You can have more than one image inside the ```<figure>``` element as long as they all share the same caption.

```<figcaption>``` The ```<figcaption>``` element has been added to HTML5 in order to allow web page authors to add a caption to an image.
Before these elements were created there was no way to associate an ```<img>``` element with its caption.

1. The ```<img>``` element is used to add images to a web page.
2. You must always specify a src attribute to indicate the
source of an image and an alt attribute to describe the content of an image.
3. You should save images at the size you will be using them on the web page and in the appropriate format.
4. Photographs are best saved as JPEGs; illustrations or logos that use flat colors are better saved as GIFs.



# colors 


1. rgb values These express colors in terms of how much red, green and blue are used to make it up. For example: rgb(100,100,90).
        1. RGB Values Values for red, green, and blue are expressed as numbers between 0 and 255.
        ![](https://negliadesign.com/wordpress/assets/RGB-color-swatches-R-700x342.jpg)

2. hex codes These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash #sign. For example: #ee3e80
        1. Hex Codes Hex values represent values for red, green, and blue in hexadecimal code.
        ![](https://i.ytimg.com/vi/c56x1aj2CPA/maxresdefault.jpg)

3. color names There are 147 predefined color names that are recognized by browsers. For example:DarkCyan
        1. Color Names Colors are represented by predefined names. However, they are very limited in number.
        ![](https://codepen.io/adevade/pen/dzqlJ/image/large.png)

> Hue is near to the colloquial idea of color. Technically speaking however, a color can also have saturation and brightness as well as hue.

> Saturation refers to the amount of gray in a color. At maximum saturation, there would be no gray in the color. At minimum saturation, the color would be mostly gray.

> Brightness (or "value") refers to how much black is in a color. At maximum brightness, there would be no black in the color. At minimum brightness, the color would be very dark.

7. Color not only brings yours  ite to life, but also helps convey the mood and evokes reactions.
1. There are three ways to specify colors in CSS: RGB values, hex codes, and color names.
2. Color pickers can help you find the color you want.
3. It is important to ensure that there is enough contrast between any text and the background color (otherwise people will not be able to read your content).
4. CSS3 has introduced an extra value for RGB colors to indicate opacity. It is known as RGBA.
6. CSS3 also allows you to specify colors as HSL values, with an optional opacity value. It is known as HSLA.


# text 

![type](https://lh3.googleusercontent.com/OML_bfx_mRWFhemUATjihMUEDXaIIeFMd7zSktVFuBiIyzIZ5njdMh5lHWu_SrZ4pH5pa2obGWZvw2Cof9nnwFmU2KOQ2PlhtHNNc0i8A5fj_IuuYcceGWUvS0ZH5OoQ6eQLWSD-EJRXw-8VkMuEIWIJK3pYmLLe27FB5sJC4ng3R00WZTLWg63QsXe8EZUoMMZDNAQVg0zjd6M5AdznhIu9cprw22cIQQurNSLjh-gA0tyBmzvDi8NyricYdPzMyZU53br1l6Bfo29aTZMGP7gZHeDyJaw2YRuS0PjSEclHYrEgJH6e-9EG-g1eYWgKZT3qVOGI96_3AHPpqPk7HlqAzdEvzry5fYp5ZprOYo604kD0Vf8B4cOnLkqOKr4wDji-izPcybwRFEjbuBPTVJqqY72DXtUO6gDjKuEANnW0zwwFu3wYzTVvb78KSJ-F-DLO-endtibClMfUTkoRasH-NzpYUG8tR-sNkklEM-hvg8nfNv3nZTGb0aU_lIe_Pmg-kz1FCVL3uGoXbGo4v8F5h5o9w3m6UKoCf1ENdvTebCP8DDuRcwjpPbfyrssWXN1kBnnUSiNXV0i0yROOAJAONKGClfXztwK-w6E-p4Gaz2WWqUFX57pNQXKSK9zv_xaKSyM6j8atlhL-OmdkmoPXAzt9ExWjFrzGRL9wTtuuG2WS-q5R7Cousnkw=w328-h375-no?authuser=0)


1. There are properties to control t  he choice of font, size, weight, style, and spacing.
2. There is a limited choice of fonts that you can assume most people will have installed.
3. If you want to use a wider range of typefaces there are several options, but you need to have the right license to use them.
4. You can control the space between lines of text, individual letters, and words. Text can also be aligned to the left, right, center, or justified. It can also be indented.
5. You can use pseudo-classes to change the style of an element when a user hovers over or clicks on text, or when they have visited a link.

> Text property 
* font-weight
* font style 
* text-transform
* text-decoration
* line height
* text-align
* vertical-align
* text-indent
* text-shadow
 and many many more 

