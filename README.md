### The Why

---

Document Text Recognition is one of the used features of the Envision App and Glasses. We process millions of document text recognition requests a month, and users read a variety of documents — letters, textbooks, reciepts, etc. with Envision. 

One of the most requested features from users is to help them identify interesting regions in a document — headings, columns, tables, etc. Envision already does this in some instances and they work online. Going forward, Envision would want to build a single endpoint that detects all these regions of interest within a document and lay them out in an accessible way for our blind and visually impaired users. 

### The Assignment

---

This is a typical problem you'll face as a Computer Vision Engineer at Envision. We'd like you a build an algorithm/model that detects headings in the test set in this repo given the OCR and bounding box output. 

The algorithm can tailored to work with only the images that are provided. Your final result can be in the form of an executable Open-CV based Python/C++ script or be deployed as a Flask Web Server. For the sake of simplicity, we'll ignore all the other layout information within the image, such as columns, etc. unless you think that would be helpful in solving the problem.

The script accepts an image and returns the headings found in the image. Below is a sample of how the Python script could work.

Note: You can also take a deep learning approach to solve this problem. If you're taking this approach then please implement it using a Jupyter Notebook and push that instead.

```
python detect_headings.py --image="/Users/EnvisionDev/test.jpg"

Heading 1
Heading 2
Heading 3
```

### Deadline

---

There's no official deadline for this assignment and the emphasis here is on the core algorithm versus code quality, etc. You can also submit the final task as a Jupyter Notebook as well. 

### Submission

---

Fork this repo and push your changes to the forked repo(please keep the repo private). Once you're done please send me the link.
