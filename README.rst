=====       
Mergeable mixins
=====

mergeable mixins adds support to use of mixins in Django models or other 
types of classes.    
The key idea here is that it removes the attribute lookup problem of the 
multiple inheritance, and let you choose from what mixin you want to copy 
functionalities

Quick start.

You can just copy paste the contents of the __init__.py where you want to
use, or you can install the package to use with more projects, below is a
quick tutorial.

1. Install the package by calling 
    
    python setup.py install

2. Import decorator wherever you want to use:

    from mergeable_mixins import merge_mixins

3. Decorate the classes you want to mix, passing a list of mixins:

    @merge_mixins(Mixin1, Mixin2)
    class GreatAndComplexBusinessLogic():
    ...

