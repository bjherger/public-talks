# Publishing a package

Based on [Cheat sheet: Publishing a Python Package](https://www.hergertarian.com/cheat-sheet-publishing-a-python-package)

## Meta

 - Audience: Familiar w/ Python, maybe familiar w/ ML
 - Have used packages
 - Probably haven't written packages

## Outline

### Intro

 - Batteries included (https://xkcd.com/353/)
 - But not on the package writing side
 
### Normal workflow

 - Design and scope your project
 - Write some awesome code
 - Structure your project for PyPI release
 - Release your project
 - The world is a wonderful place

#### Cheat sheet

 - Design and scope your project
   - Actually whiteboard out modules, classes and functions
 - Write some awesome code
   - Choose a documentation format such as rST
   - Write a README
 - Structure your project for PyPI release
   - Pray and spray
   - Create a Setup.py file
   - Write unittests (bonus points!)
 - Release your project
   - Package everyting
   - Upload to PyPI
   - Set up Continuous Integration (bonus points 2x!)
 
### A few choices to look at & general ramblings

 - The other side of package management (https://xkcd.com/1987/)
 - Package writing is not batteries included
 - Multiple ways to generate documentation
 - Imitation is the sincerest form of flattery: Choose a template (or example project), and copy them. To death. 

### Recap

 - Python is a batteries included language
   - Except for when you're the one building toys
 - The process isn't difficult, but also isn't well documented
 - Imitation is the sincerest form of flattery
