Name: Stenography
Description: The user is provided with a GIF image and a description, perhaps something like "There's always a troll hidden somewhere.".

How to Solve:

Upon inspection with a hex editor and some research about the GIF file format, the user should find that the ending tag for GIF is 00 3B or " ;" however there is some data after the last occurrence of 00 3B. The user should then look into the information right after the last occurrence of 00 3B and upon finding that information should find the JFIF tag. When researching the JFIF tag, they will find that it belongs with a JPEG image, and should then try extracting the data out into its own file which will then open and have the flag. 

What to distribute: ./dist/magnetism.gif

something.jpg is the file they will extract from the end of magnetism.gif.

Key: MCA-E3F2ABEC