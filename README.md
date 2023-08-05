# beautifulsoup4-docs
bs4 / beautifulsoup4 docs example generated by sphinx-autoapi + furo theme

<img width="1440" alt="Screenshot 2023-08-05 at 13 56 31" src="https://github.com/cmdlineluser/beautifulsoup4-docs/assets/99486669/26ff0f77-d221-40d0-962a-b5f2a8b85d85">

Created with https://github.com/readthedocs/sphinx-autoapi

    python3 -m pip install sphinx sphinx-autoapi furo

    wget https://www.crummy.com/software/BeautifulSoup/bs4/download/4.12/beautifulsoup4-4.12.2.tar.gz
    tar xf beautifulsoup4-4.12.2.tar.gz

    cd beautifulsoup4-4.12.2/

I then ran:

    sphinx-quickstart docs

I then edited `docs/source/conf.py` to use autoapi and the `furo` theme:

    extensions = ['autoapi.extension']
    autoapi_dirs = ['../../bs4']

    html_theme = 'furo'


I then ran:

    sphinx-build -b html docs/source docs/build

This then creates `docs/build/index.html`