# DinoHide
Homebrew pixel value differencing algorithm.
#                         .       .
#                        / `.   .' \
#                .---.  <    > <    >  .---.
#                |    \  \ - ~ ~ - /  /    |
#                 ~-..-~             ~-..-~
#             \~~~\.'                    `./~~~/
#   .-~~^-.    \__/                        \__/
# .'  O    \     /               /       \  \
#(_____,    `._.'               |         }  \/~~~/
# `----.          /       }     |        /    \__/
#       `-.      |       /      |       /      `. ,~~|
#           ~-.__|      /_ - ~ ^|      /- _      `..-'   f: f:
#                |     /        |     /     ~-.     `-. _||_||_
#                |_____|        |_____|         ~ - . _ _ _ _ _>
#

---INDEX---------------------------------------------------------------------------------------------------------

FILES:

1. Stegosaurus		- python script 	- simple pvd hiding/extraction
2. broken_Stegosaurus 	- python script 	- multiway pvd hiding/extraction !!produces incorrect output!! 


---USING Stegosaurus---------------------------------------------------------------------------------------------

<message_file> must be utf-8 encoded
<cover_image> & <stego_image> must be 24-bit .png

HIDING:	'-e'
	
	SYNTAX: 	'<python invocation> Stegosaurus.py -e <message_file> <cover_image> <stego_image>'
	EXAMPLE:	'py Stegosaurus.py -e message_file.txt cover_image.png stego_image.png'

EXTRACTION: '-d'

	SYNTAX: 	'<python invocation> Stegosaurus.py -e <stego_image> <output_file>'
	EXAMPLE:	'py Stegosaurus.py -d stego_image.png output_file.txt'

ANY OTHER USE WILL THROW ERRORS


---USING broken_STEGOSAURUS--------------------------------------------------------------------------------------

<message_file> must be utf-8 encoded
<cover_image> & <stego_image> must be 24-bit .png

HIDING:	'-e'

	SYNTAX: 	'<python invocation> broken_Stegosaurus.py -e <message_file> <cover_image>'
	EXAMPLE:	'py broken_Stegosaurus.py -e message_file.txt cover_image.png'

EXTRACTION: '-d'

	!!PRINTS SLICE OF DECODED MESSAGE TO THE SCREEN!!
	!!DOES NOT PRODUCE CORRECT OUTPUT!! 

	SYNTAX: 	'<python invocation> broken_Stegosaurus.py -d <stego_image> <output_file>'
	EXAMPLE:	'py broken_Stegosaurus.py -d stego_image.png output_file.txt'

ANY OTHER USE WILL THROW ERRORS
