# py4ds
Setup an Awesome Python Environment for Data Science

<h2>Introduction</h2>
Coding in Python is awesome and is getting more awesome with every new release! For me, this is mainly due to the massive amount of freely available libraries, its readability, and the recently introduced type annotations. However, especially we as Data Scientists tend to often produce big and messy Jupyter notebooks or python files that are hard to follow. Apart from that, we often run into version clashes when one project depends on a different version fo the same library. Fixing this takes too much time and often leads to issues with other projects. There must be a way to avoid that and facilitate our lives. In this article, I will go through the tools that I use and the techniques that I usually follow. This hopefully will help future me to remember all of that, and more importantly, will help you also learn something helpful. Without further ado, let’s get our hands dirty.
<br>
<h2>The Python Environment</h2>
<h3>The Interpreter</h3>
Let’s get started with the most important thing when working with python: the interpreter. For sure you could just simply download and install your favorite version of python and put everything into that. But what if you have programs that require different python versions or programs that depend on different versions of the same third-party module and you want to switch between those programs seamlessly?
Pyenv will help you doing that!
Pyenv is a set of three tools, from which I present two here, that are pyenv (used to install python) and pyenv-virtualenv (used to configure your global tools). You can install them by

<code>curl https://pyenv.run | bash</code><br>
After that, add the following lines to your .bashrc (same for .zshrc) to have pyenv available in your terminal<br>
<code>
export PATH="~/.pyenv/bin:$PATH"
eval "$(pyenv init -)"
eval "$(pyenv virtualenv-init -)"
</code><br>
and finally, restart your terminal. Now, you can use pyenv to install almost any python interpreter, including pypy, and anaconda. Note, that pyenv builds python locally on your machine. Building python requires several libraries. On my Ubuntu machine, I have to install the following ones to not run into problems
<p>
<code>
sudo apt-get install build-essential libsqlite3-dev sqlite3 bzip2 libbz2-dev zlib1g-dev libssl-dev openssl libgdbm-dev libgdbm-compat-dev liblzma-dev libreadline-dev libncursesw5-dev libffi-dev uuid-dev
</code>
</p>
<br>
<br>
<source><a href="https://towardsdatascience.com/how-to-setup-an-awesome-python-environment-for-data-science-or-anything-else-35d358cc95d5">Setup an Awesome Python Environment for Data Science</a></source>
