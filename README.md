Python Packages

This course will use a handful of third-party packages:

    pytest
    pytest-cov
    pytest-html
    pytest-xdist
    requests
    playwright

These packages are not part of the Python Standard Library. They must be installed separately using pip, the standard Python package installer. You can install them all before you create your test project, or you can install them as you complete each chapter in the course.

To install each package, enter `pip install <package-name>` at the command line. For example: `pip install pytest`. If you already have a package installed but need to upgrade its version, run `pip install --upgrade <package-name>`.

Running pip install will install the pytest package globally for the whole system. Installing Python packages globally is okay for this course, but it typically isn't a best practice in the "read world." Instead, each project should manage its own dependencies locally using a virtual environment. Virtual environments let projects avoid unnecessary dependencies and version mismatches.

Running Tests

To run the example tests from the command line, run python -m pytest from the project root directory. This command will discover and run all tests in the project.

You can also run tests using the shorter pytest command. However, I recommend always using the lengthier python -m pytest command. The lengthier command automatically adds the current directory to sys.path so that all modules in the project can be discovered.
