
# Generate/parameterize verilog files using mako templating and python

At work, we had a large spreadsheet of 140+ instructions, signals, opcodes, and comments that needed to be turned into a decoder and other things, so instead of manually creating the verilog files, I used a python script and mako to generate them. It was pretty easy and straightforward to do, so I made this guide to share the basics of how to use mako to save yourself some time.


## Mako Templates for Python

Mako is a template library written in Python. It provides a familiar, non-XML syntax which compiles into Python modules for maximum performance. Mako's syntax and API borrows from the best ideas of many others, including Django and Jinja2 templates, Cheetah, Myghty, and Genshi. Conceptually, Mako is an embedded Python (i.e. Python Server Page) language, which refines the familiar ideas of componentized layout and inheritance to produce one of the most straightforward and flexible models available, while also maintaining close ties to Python calling and scoping semantics.


## Doing the thing
### Parameterizing instances
If you have an instance that you want to generate 'n' times, you can do so by creating a file, like parameterize_inst.v.mako, that looks something like this:






## Run Locally

To run, cd to the directory containing example.v.mako, and enter:

```bash
  python3 mako_python.py > mako_python.v
```




