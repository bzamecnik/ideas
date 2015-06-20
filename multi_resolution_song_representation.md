# Multi-resolution representation of songs

Musical songs typically contain a lot of repeating or similar pattern - variation of a few basic themes. Those variation could be factorized to some basic part and a difference. Thus the information redundancy would be lowered.

"How a musician can remember so much notes?" He just remembers the themes and variations and can synthesize the individual notes.

It is a similar process to lossy JPEG compression - projection on a basis and removing less important coefficients.

Then we could do a lot of interesting things:

- remove details - ornaments, variations
    - create an "easy version"
    - continuously
- amplify details
- see what are the important parts and what are details
