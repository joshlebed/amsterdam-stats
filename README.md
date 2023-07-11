# amsterdam-stats

generate reports from amsterdam billiards stats page

## user guide

### prereqs

- [python 3.10](https://www.python.org/downloads/release/python-31010/) installed locally
- `.env` file in the root directory with your username and password for http://leagues2.amsterdambilliards.com/
  - copy `.example.env` from this directory into a new file `.env` in the same directory and add your `id` and `secret`

### steps

- in this directory, run:

```bash
python3.10 -m venv .venv  # create python virtual environment
source .venv/bin/activate  # activate virtual environment
pip install -r requirements.txt  # install dependencies

# run script
python amsterdamstats/amsterdamstats.py
```

## dev quickstart

one time setup:

```bash
python3.10 -m venv .venv
```

activate python virtual environment and update dependencies (after each pull):

```bash
source .venv/bin/activate
pip install -r requirements.txt -r requirements-dev.txt
```
