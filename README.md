# XGBoost explainability

## Setup
1. Install [Vagrant](https://www.vagrantup.com/)
1. In a console change to the repository folder
1. Edit the memory / cpu settings and the forwarded port (8888) in `Vagrantfile` if necessary
1. Run `vagrant up` (takes a while, likely 30min+)
1. SSH into the virtual machine with `vagrant ssh`
1. Set `Jupyter` password with `jupyter notebook password`

## Running the Jupyter notebook
1. Change into the `jupyter` folder
1. Start Jupyter notebook server with `jupyter notebook`
1. Open browser at [http://localhost:8888/](http://localhost:8888)

## Presenting the Jupyter notebook as slide show
1. Change into `jupyter` folder
1. `jupyter nbconvert Explainability\ of\ XGBoost\ vs\ LIME.ipynb --to slides --reveal-prefix lib/reveal.js --post serve --ServePostProcessor.ip='0.0.0.0'`
1. Open browser at [http://localhost:8889](http://localhost:8888)
