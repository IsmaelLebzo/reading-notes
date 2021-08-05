# HTML & CSS by JON DUCKETT Part V
![HTML & CSS](https://www.sharptutorial.com/wp-content/uploads/2018/12/html-gif-9.gif)
## Images
There are a variety of reasons why you would wish to put an image on a web page, including a logo, photograph, illustration, diagram, or chart.

When choosing and creating pictures for your website, there are numerous factors to consider, but spending the time to get them properly can make it appear more appealing and professional.
This chapter will teach you how to:
- Include an image in your web pages using HTML
- Pick which image format to use
- Show an image at the right size
- Optimize an image for use on the web to make pages
load faster

### Choosing Images for Your Site

A picture is worth a thousand words, and outstanding graphics may help distinguish between an average-looking site and one that is truly engaging.

Images should...
- Be relevant
- Convey information
- Convey the right mood
- Be instantly recognisable
- Fit the color palette
### Storing Images on Your Site
If you're starting from scratch, it's a good idea to make a folder for all of the photos you'll need.

## Color
Color can really bring your pages to life.
In this chapter we will look at:
- How to specify colors, as there are three common ways in
which you can indicate your choice of colors (plus extra
ways made available in CSS3)
- Color terminology, as there are some terms that are very
helpful to understand when it comes to picking colors
- Contrast, and ensuring that your text is readable
- Background color

When it comes to looking at the colors of text and boxes in CSS, everything you learn about colors in this chapter will be applied in later chapters.

### Foreground Color

The color property allows you
to specify the color of text inside
an element. You can specify any
color in CSS in one of three ways:

rgb values:

These express colors in terms
of how much red, green and
blue are used to make it up. For
example: rgb(100,100,90)

color names:

There are 147 predefined color
names that are recognized
by browsers. For example:
DarkCyan

hex codes:

These are six-digit codes that
represent the amount of red,
green and blue in a color,
preceded by a pound or hash #
sign. For example: #ee3e80

### Understanding Color
Every color on a computer screen is made by combining red, green, and blue in various proportions. You may use a color picker to find the color you desire.

### CSS3: HSL Colors
Using hue, saturation, and lightness values, CSS3 offers a completely new and straightforward approach to describe colors.
Like the HUE.

## Text
The characteristics that govern the look of text may be divided into two categories:

- Those that directly affect the font and its appearance
(including the typeface, whether it is regular, bold or italic,
and the size of the text)
- Those that would have the same effect on text no matter
what font you were using (including the color of text and
the spacing between words and letters)

The way you style your content has a big impact on how legible your pages are. While we're going through these attributes, I'll offer you some design advice on how to present your type.

### Typeface Terminology
1. Serif:

Serif fonts have extra details on
the ends of the main strokes of
the letters. These details are
known as serifs.

2. Sans-Serif:

Sans-serif fonts have straight
ends to letters, and therefore
have a much cleaner design.

3. Monospace:

Every letter in a monospace (or
fixed-width) font is the same
width. (Non-monospace fonts
have different widths.)

### Size of Type
The font-size attribute allows you to set the font's size. A font's size can be specified in a variety of ways. The following are the most common:

1. pixels
2. percentages
3. ems
____

# JPEG vs PNG vs GIF

![JPEG vs PNG vs GIF](https://dt2sdf0db8zob.cloudfront.net/wp-content/uploads/2019/05/GIF-vs-JPG-vs-PNG.jpg)

There are hundreds of picture formats to choose from, each with its own set of applications. I'm guessing that most of us haven't come across 90% of the picture formats mentioned in Wikipedia.

## TL;DR
All photos that feature a natural scene or snapshot with smooth color and intensity change should be saved in JPEG format. Use PNG for any picture that requires transparency, as well as images containing text and objects with sharp contrast borders, such as logos. For pictures with animations, use the GIF format.
## Compression
Almost all types of data we encounter on the internet — text, picture, video, and so on — are compressed to decrease data size and speed up transmission. The size of an image is mostly determined by the format and compression used.
## Transparency
- JPEG: images don’t support transparency and are hence not usable for such cases.
- PNG: Transparency may be achieved in pictures in two ways: by introducing an alpha channel that permits partial transparency or by designating a single color translucent (index transparency). The edges merge seamlessly into the backdrop thanks to partial transparency. Only index transparency is supported by PNG8 pictures (explained in the "Colours" section below), whereas alpha channel transparency is supported by PNG24 images.
- GIF:Transparency is enabled in pictures by defining a single color in the color palette as transparent (index transparency). The edges (especially rounded or over-detailed edges) suffer from a bad jagged appearance due to the lack of partial transparency. Though this may be mitigated to some level by dithering, GIF is inappropriate for pictures with translucent backgrounds, especially with better PNG support.

### Colours
JPEG pictures have a color range of about 16 million. This is what makes them ideal for storing natural-scene photos.

PNG pictures are divided into two types: PNG8 and PNG24. PNG8 can manage up to 256 colors, but PNG24, like a JPEG picture, can accommodate up to 16 million colors. Use PNG8 for basic forms with fewer colors, and PNG24 for complicated logos and shapes with rounded edges on a transparent backdrop in excellent resolution.

The number of colors in a GIF image is restricted to 256. If index transparency is utilized, one of these 256 colors is designated as transparent, leaving the remaining 255 for other use.