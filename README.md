object_by_name
==============
Get an object by name or dotted path, import if it necessary.

Install
-------
    pip install object_by_name

Usage
-----
    >>> from object_by_name import object_by_name

    >>> object_by_name('test_package')
    <module 'test_package' from ...>

    >>> object_by_name('test_package.test_module')
    <module 'test_package.test_module' from ...>

    >>> object_by_name('test_package.test_module.TestClass')
    <class 'test_package.test_module.TestClass'>

    >>> object_by_name('test_package.test_module.instance')
    <test_package.test_module.TestClass object at 0x...>

    >>> object_by_name('test_package.test_module.instance.method')
    <bound method TestClass.method of <test_package.test_module.TestClass ...>>