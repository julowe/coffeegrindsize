# Coffee Grind Size Application

This is a pared down copy of [jgagneastro's coffeegrindsize repo](https://github.com/jgagneastro/coffeegrindsize). No, this is a hack and not a fork because that repo is 400mb. So I am copying in files to this repo and adding in the 4/3 factor for volume calculation from [wannabecoffeenerd's unmerged pull request](https://github.com/jgagneastro/coffeegrindsize/pull/11).

I am running linux so just wanted to simply run the `coffeegrindsize.py` file.


## Running the application

I used a python virtual environment (venv) to run this application. For Ubuntu 22.04.2 LTS you should already have python3 installed, along with venv and tkinter. i.e. run:

```
apt install python3.10-venv
apt install python3-tk
```

Go to your local copy of this repo, run `python3 -m venv venv-coffee` to create a venv called `venv-coffee`. Then use/activate the venv with `source venv-coffee/bin/activate`. Then install the requirements for the application using the requirements file I made with the command `python3 -m pip install -r requirements.txt`. Run the application with `python coffeegrindsize.py`.

If this doesn't work for some reason either start over with a new venv (run `deactivate`, then delete the directory `venv-coffee`, then repeat step to create venv. or just make a new venv with different name) or just proceed with existing venv, and install the modules it is erroring on. That is, if it gives you errors something like `ModuleNotFoundError: No module named 'PIL'` then just google the error and install that module in the venv (e.g. `python3 -m pip install Pillow` which provides the `PIL` module). If it is a different error, well... go to the original repo and see if there are any issues or pull requests that have the same errors or search online for the error messages.


## Code To Do

Collection of possible changes I am collecting as I use the app.

- [x] create a new repo and pull in only the one main .py file & LICENSE & README. 
- [ ] Shrink file size of PDFs in the Help folder and add those to repo. Intent is to make repo smaller and focused on code. Get rid of build and .pages files.
- [x] add instructions on creating venv and make a requirements file
- [ ] make gui open/save dialogs default to source folder - or at least remember last place you opened/saved to in current session
- [ ] make image window resize to resized outer container, and/or add scroll bars
- [ ] make window open smaller than the monitor resolution
- [ ] make open image dialog default to png AND jpg
- [ ] option to use data label as filename base


## Original Readme Info

The below is not relevant to this repo, but I already hate decoupling this copy of the repo from the original, so I didn't want to delete this. Go to the [original repo](https://github.com/jgagneastro/coffeegrindsize) for the below.

To open the application simply launch the .app file located at /App/dist/coffeegrindsize.app

Please see this GitHub repo developed by Chris Saterlee for OS X and Windows installation packages of the app:
https://github.com/csatt/coffeegrindsize/releases/tag/v1.0.0

Thanks a lot Chris !
