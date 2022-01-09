# Patternmaker

This is an experiment to investigate if it is possible to use vanilla js and svg in order to create a technical drawing software of sorts.
Special attention was taken to ensure that drawings would be to scale when printed so as to enable a user to create patterns for sewing or other crafts. 
The canvas can be expanded page by page horizontally and vertically.

The drawing tools are currently lacking in features. The only availiable tool is a path tool for drawing shapes. These are the controls:

while editing shape:
- left click = add point
- hold and pull left click = add curved point
- right click = stop editing shape
- ctrl click = close shape

otherwise:

while active shape:
- left click:
    - on point in active shape:
        - point becomes Point and follows mouse, 
        - if you click it stays 
        - if you click and drag it becomes a curved point
    - click & drag elsewhere: move shape as a whole
- double click on any point in active shape: edit shape
- right click
    - on point in active shape: remove point
    - elsewhere deactivate shape.

while not active shape:
- left click: create new shape.
