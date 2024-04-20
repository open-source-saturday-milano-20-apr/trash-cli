Development
-----------

Environment setup::

    virtualenv env --no-site-packages
    source env/bin/activate
    pip install -r requirements-dev.txt -r requirements.txt

Running tests::

    pytest -m 'not slow'        # run only fast tests
    pytest -m 'slow'            # run slow tests
    pytest                      # run all tests
