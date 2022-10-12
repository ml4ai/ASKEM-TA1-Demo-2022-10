# ASKEM TA-1 Working Group Demo for October 2022

## Install

Requires:

- openapi
- cryptography
- fernet

## Content

[Needs updating]

There are two demo Jupyter Notebook files.

The first was written by Clay Morrison, called
`ASKEM_TA1_demo_2022_10.ipynb`. It contains a candidate workflow and a
number of markers for groups to contribute content and code.

The second was written by Mike Cafarella, called
`ASKEM-Simple-Walkthrough-v1.ipynb`. It contains enough code to do a
simple walkthrough of TA-1 components. It will:
1. Load model source text from XDD
2. Execute the original model and show results 
3. Analyze it using Gromet
4. Load a Pandemic Ontology
5. Attempt to find locations in the model where parameters from the
   Pandemic Ontology are found in the model code.
6. Expose these recovered knobs to the user, for adjusting model
   parameters. The user can then execute the altered model and see
   results.
7. After tweaking user can choose to store the new altered model in
   XDD.

As of now, this is a cheap-and-cheerful end-to-end demo. It works, but
there are a number of placeholders where we need to do more
work.  For example, we have a hard-coded pandemic model instead of
loading or discovering it. Also, right now the gromet representation
is generated but not actually used to alter and execute the model; we
use the source code instead. Also, the model/knob discoveries are
hard-coded instead of dynamically discovered.

Finally, there are a number of places where you can and should
add your own team's work. I have not identified all of these; Clay's
file above is probably a better guide to that.

This simple walkthrough relies on a number of pretty standard Python
data science packages (shutil, requests, matplotlib, pandas, etc). The
only thing you probably have to install is the gromet package. You can
find instructions for this in the Arizona repo here:
https://github.com/ml4ai/automates.

Also, note that you'll need the latest version of plotly (5.10).


