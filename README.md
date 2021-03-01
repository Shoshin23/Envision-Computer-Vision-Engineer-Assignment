### The Why

---

Document Text Recognition is one of the used features of the Envision App and Glasses. We process millions of document text recognition requests a month, and users read a variety of documents — letters, textbooks, reciepts, etc. with Envision. 

One of the most requested features from users is to help them identify interesting regions in a document — headings, columns, tables, etc. Envision already does this in some instances and they work online. Going forward, Envision would want to build a single endpoint that detects all these regions of interest within a document and lay them out in an accessible way for our blind and visually impaired users. 

### The Assignment

---

This is a typical problem you'll face as a Computer Vision Engineer at Envision. We'd like you a build an algorithm/model that detects headings in the given test set in this repo given the OCR and bounding box output. 

For OCR, you can use Google Cloud Vision to get the OCR output and use the bounding box data provided with this repo.

The algorithm can tailored to work with only the images that are provided, these represent the most common type of images that users tend to use with Envision. Your final result can be in the form of an executable Open-CV based Python/C++ script or be deployed as a Flask Web Server.

The script accepts an image and returns the headings found in the image. Below is a sample of how the Python script could work. 

```
python detect_headings.py --image="/Users/EnvisionDev/test.jpg"

Heading 1
Heading 2
Heading 3
``` 

**Note: You can also take a deep learning approach to solve this problem. If you're taking this approach then please implement it using a Jupyter Notebook and push that instead.**

### Other Important Stuff

---

1.  For the sake of simplicity, we'll ignore all the other layout information within the image, such as columns, etc. unless you think that would be helpful in solving the problem.

2. Also for simplicity's sake, you can assume that the images passed onto the script are properly cropped documents. You don't have to concern yourself with documents/images that don't go through a cropping/perspective-transform process.

3. The emphasis for this assignment is the _core algorithm and less about code quality_. Though code quality is very much emphasised at Envision, I can understand that it might be time consuming as well at the early prototyping stage.

4. It's not mandatory to distinguish between the header types(H1, H2, H3, H4, etc.). Bonus points if you can work on distinguishing headings but that can be considered outside the scope of the implementation.

5. If you think that there are other reasonable constraints you want to take into account, please do so and make a note of them in the code/ReadMe.


### Deadline

---

There's no official deadline for this assignment and the emphasis here is on the core algorithm versus code quality, etc. You can also submit the final task as a Jupyter Notebook as well. 

### Submission

---

Fork this repo and push your changes to the forked repo(please keep the repo private). Once you're done please send me the link.
