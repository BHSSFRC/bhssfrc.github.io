New Programmer Documentation
---
revision 0

* auto-gen TOC:
{:toc}

## Getting Started
### Installing tools
1. Install [`git`.](https://git-scm.com/)
 * If you want, you can also install a [GUI interface for it.](https://git-scm.com/downloads/guis) As a new user, you may find [GitKraken](https://www.gitkraken.com/) to be the easiest to work with. **Avoid the GitHub client like the plauge.**
2. Install the [JDK](http://www.oracle.com/technetwork/java/javase/downloads/index.html) for your operating system. If you don't know what that is, it's most likely Windows, 64 bit.
3. Install your Java IDE of choice. Suggestions:
 * [Eclipse](https://www.eclipse.org/)
 * [IntelliJ IDEA](http://www.jetbrains.com/idea/)<br>Note: the Community Edition is fine, but you can apply for a free copy of the Ultimate edition as a student.
 * [VS Code](https://code.visualstudio.com/) with the [Java](https://marketplace.visualstudio.com/items?itemName=redhat.java) and [Gradle](https://marketplace.visualstudio.com/items?itemName=cazzar09.Gradle) extensions.

### Prepare `git`
#### Set up GitHub
##### If you already have an account:
1. Pester me to get into the [GitHub organization.](https://github.com/BHSSFRC) This will give you read and write access to all of the code as it is stored online.
2. For the love of denim jackets: [SET. UP. 2FA.](https://help.github.com/articles/securing-your-account-with-two-factor-authentication-2fa/) This will make it that much harder for someone to worm thier way into your account.
 * If you do this, and didn't install a GUI like GitKraken, you'll need to install SSH and set up a key for it on GitHub (as HTTP remotes won't work the same way for 2FA users.)
3. Sign up for the [student pack](https://education.github.com/pack) if you haven't already for all sorts of free stuff.
4. ~~Gloat, because everyone else is going to have much more to do in this part.~~

##### If you don't:
1. Register for an account at [GitHub](https://github.com), using an email that MCCSC did **not** give you. MCCSC emails will not recieve the confirmation email from GitHub, because MCCSC is silly.
2. Gain access to the [GitHub organization.](https://github.com/BHSSFRC)
3. [Set up 2FA](https://help.github.com/articles/securing-your-account-with-two-factor-authentication-2fa/) ~~to keep the Russians out.~~
4. [Get a ssh key configured for your account.](https://help.github.com/articles/connecting-to-github-with-ssh/)
5. Sign up for the [student pack](https://education.github.com/pack) because you deserve free stuff.
 
#### Set up `git` itself.
Now `git` needs to know who you are, for various reasons (prime among them being so you can be properly credited for your contributions with green squares.)

First, set your name.

```sh
git config --global user.name "Your name goes here!"
```

Then, your email. This **must** be the same email that you have on your GitHub account.

```sh
git config --global user.email "your_email@place.tld"
```

You can test these values by doing `git config --global user.name` (or `user.email`.)
### Get a copy of the code
You'll need to "clone" the code from GitHub. This can be done with a simple command if you're not using a GUI.

```sh
cd /path/where/you/want/the/code/
# personal reccomendation: ~ on Linux/Mac, C:\Users\yourusername on Windows
git clone git@github.com:BHSSFRC/repo-to-be-announced.git
```
(This command will only work if you configured an SSH key for your GitHub account.)

You should now see a folder named `repo-to-be-announced` in the directory you ran the `git clone` command in.
