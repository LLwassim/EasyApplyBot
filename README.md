# LinkedIn Easy Apply Bot

Automate your LinkedIn job applications using Easy Apply feature with ease using this Python and Selenium-based bot.
Tested successfully on over 50,000+ job applications!

## Disclaimer

**Use this bot at your own risk.** This bot comes with no warranties or guarantees. I am not liable for any
consequences, including potential account restrictions or suspensions by LinkedIn. Consider it an educational and
exploratory project!

## Credits & Enhancements

This repository is a fork from the original developer [Nathan Duma](https://github.com/NathanDuma), with significant
code updates contributed by [Micheal Dingess](https://github.com/madingess/) and [taimur](https://github.com/voidbydefault/)

I have cloned this project and updated it to the latest selenium and chromdriver versions to ensuring funtionality it is up to date as of 9/12/23.

## 🎥 How-to Video

Setting-up the bot:

- For your convenience, [taimur](https://github.com/voidbydefault/) has created a comprehensive video tutorial to guide you through the setup and usage of the bot.
  Check it out on [YouTube](https://youtu.be/IXflenwJzhQ).

Setting-up the optional monitoring dashboard (Sep-23 update):

- If you wish to setup the optional bot monitoring dashboard using PowerBI then watch [this YouTube video.](https://youtu.be/4LH8WTrMCxw)

## 🛠️ Setup & Launch

If you are new to Python, please watch this [video first](https://youtu.be/IXflenwJzhQ).

1. Start by configuring the `config.yaml` file. This is a one-time setup and contains the necessary inputs for running
   the bot. Necessary help is documented within the `config.yaml`. Please maintain the formatting and avoid adding
   unnecessary spaces in the file.
2. After configuring the file, install the dependencies listed in `requirements.txt`.

3. Now, you're ready to launch the bot using your preferred method:

   - If you're using an IDE like PyCharm Community Edition, execute `main.py` from your IDE (recommended)
   - If you prefer the command line or terminal, activate the virtual environment with `source venv/bin/activate`, then
     run `python3 main.py`.

In case you encounter any "dependencies not found" errors, ensure that the required dependencies are installed. You can
verify this using your IDE or, if you're using the command line/terminal, run `pip install -r requirements.txt` before
executing `python3 main.py` to initiate the bot.

### 🐞🔧 Known Issues & Resolutions

1. In some cases, integrated development environments (IDEs) such as PyCharm might conflict with the included virtual
   environment (venv) in this project. To address this, you can delete the `venv` folder and configure the Python
   interpreter to use the "local" option. Furthermore, installing the dependencies from `requirements.txt` ensures a
   successful run of `main.py`.

2. The bot occasionally struggles with providing accurate or complete responses to questions in non-English job posts,
   leading to potential infinite loops. The solution is to close such a job, allowing the bot to progress to the next
   item in the queue.

3. If bot is stuck in a weird one-off question, then simply click on [x] to close the job application. Bot will proceed
   to next job in the queue.
4. Some employers add human checks like enter the sum of 2 + 7 (or x + y) and other really one-off questions. The bot
   cannot be trained to answer those questions. It is suggested to add such employers to the `companyBlacklist:` in
   `config.yaml` so the bot continues its job without hindrance.

## 🆘❓Need Further Assistance?

If you're new to Python, I recommend watching the [YouTube](https://youtu.be/IXflenwJzhQ) video for a comprehensive
overview. If you encounter any genuine issues with the code or the bot's functionality, please raise them in the "
Issues" section of this repository. However, please refrain from using issues for personal technical support.

For general inquiries and support, feel free to post a comment describing your problem under
the [YouTube](https://youtu.be/IXflenwJzhQ) video or messaging me directly.
