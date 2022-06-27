# jupyter-dashboard-example
Jupyter Dashboard Example

All copied from:

https://mljar.com/blog/dashboard-python-jupyter-notebook/

## What I did...

```
cd jupyter-dashboard-example/
python -m venv djenv
source djenv/bin/activate
vi requirements.txt
pip install -r requirements.txt
# add kernel
python -m ipykernel install --user --name djenv
jupyter notebook --allow-root --ip=0.0.0.0
```

Then go to:

http://192.168.50.70:8888/tree

Create notebook in `djenv` kernel and add code from web-page above.

Include YAML in first cell - NOTE: Jupyter cannot execute this - but Mercury will use it ;-)

Run mercury:

```
mercury run 0.0.0.0:8000
```

View the results at:

http://192.168.50.70:8000/app/2

or:

http://192.168.50.70:8000
