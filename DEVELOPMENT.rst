Development
-----------

Environment setup::

    python -m venv .venv
    source .venv/bin/activate
    pip install -r requirements-dev.txt -r requirements.txt

    tox &&
    scripts/test-sdist &&
    scripts/check-types

Running tests::

    pytest -m 'not slow'        # run only fast tests
    pytest -m 'slow'            # run slow tests
    pytest                      # run all tests


Run test on all multiple python versions::

    brew install pyenv
    pyenv install 2.7.18
    pyenv install 3.10

pyenv install