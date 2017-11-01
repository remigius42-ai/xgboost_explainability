# XGBoost explainability

## Setup
1. Install [Vagrant](https://www.vagrantup.com/)
1. In a console change to the repository folder
1. Edit the memory / cpu settings and the forwarded ports (8888, 8889) in `Vagrantfile` if necessary
1. Run `vagrant up` (takes a while, likely 30min+)
1. SSH into the virtual machine with `vagrant ssh`
1. Set `Jupyter` password with `jupyter notebook password`

## Running the Jupyter notebook
1. Change into the `jupyter` folder
1. Start Jupyter notebook server with `jupyter notebook`
1. Open browser at [http://localhost:8888/](http://localhost:8888)
1. Open the notebook `XGBoost explainability.ipynb`

## Presenting the Jupyter notebook as slide show
The cells in the notebook feature a slide show configuration, which can be inspected with the
menu entry `View -> Cell Toolbar -> Slideshow`.

For presenting the notebook as slide show, you may either use [RISE](https://damianavila.github.io/RISE/index.html)
or the built-in slide conversion with `nbconvert`. RISE features live cell evaluation and seems to cause less issues
in Chrome, while `nbconvert` supports speaker notes with the local `reveal.js` installation.
### Using RISE
1. Open browser at [http://localhost:8888/](http://localhost:8888)
1. Open the notebook `XGBoost explainability.ipynb`
1. Switch to the live slide show mode by pressing `Alt+R` or by clicking the button in the toolbar (on the far right)
### Using the built-in conversion with `nbconvert`
1. Change into `jupyter` folder
1. `jupyter nbconvert XGBoost\ explainability.ipynb --to slides --reveal-prefix lib/reveal.js --post serve --ServePostProcessor.ip='0.0.0.0'`
1. Open browser at [http://localhost:8889](http://localhost:8889)
