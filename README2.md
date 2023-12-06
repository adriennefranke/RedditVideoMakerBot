# From Scratch
- Install VS Code: https://code.visualstudio.com/
- Make Github account: https://github.com
- Make an SSH key
- Install Git
	- `git --version` - This should prompt you to install Git
	- Git is for version control. It's how you pull down and push up code changes
	- https://git-scm.com/book/en/v2/Getting-Started-Installing-Git
- Install Python
	- Install `pyenv` - this is what you'll use to manage different versions of Python
	- `pyenv install 3.10` - the app needs some version of Python 3.10
	- `pyenv local 3.10` - this sets the local version of Python to be 3.10
	- `python --version` - you should see `Python 3.10` printed out in your console
- Create a virtual environment
	- https://docs.python.org/3/library/venv.html#creating-virtual-environments
	- A virtual environment is a place where you can install specific packages necessary to run your program. When your virtual environment is activated, all the Python things you install will only be installed in your virtual environment
	- `python -m venv ./venv`
	- To activate: `source venv/bin/activate`
- Clone repo
	- Cloning the repo is when you basically download the code from a repository
	- Once you've cloned something, you can push and pull from the main branch
	- `ssh link-to-repo`
- Install pip
	- Pip is a package manager. You use it to install Python packages
	- Install it globally
	- `python -m ensurepip --upgrade`
	- https://pip.pypa.io/en/stable/installation/#ensurepip
- Install requirements
	- Might need to install `homebrew`
	- Might need to use `homebrew` to install `ffmpeg`
	- May need to adjust linux ffmpeg function to install via brew
- Set up Reddit API
	- You can add "https://localhost:8000" as the redirect URL
- Other fixes
	- Probably need to `pip install py3-tts`
	- https://github.com/thevickypedia/py3-tts
	- Need to install `brew install portaudio` & `pip install pyaudio`
- TikTok TTS
	- Follow these instructions to get TikTok Session ID: https://github.com/elebumm/RedditVideoMakerBot/pull/1252
	- https://github.com/Steve0929/tiktok-tts
	- Replace `TikTok.py` with this code: https://github.com/elebumm/RedditVideoMakerBot/issues/1858#issuecomment-1808631802
- 

## Instructions to Run
1. Open terminal
2. Type `cd dev/RedditVideoMakerBot`
3. Type `source venv/bin/activate`
4. Type `python main.py`

To open the code and change your configuration:
1. Make sure you are in `RedditVideoMakerBot`
2. Type `code .` This opens the code in VS Code
3. Open the file `config.toml` and make your changes and save your file
4. Re-run the program (`python main.py`)