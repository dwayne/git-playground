# Git Playground

Play with the latest Git in a virtual machine.

# Usage

```sh
# If you have Git installed then
$ git clone
# Otherwise
$ mkdir git-playground && curl -L https://github.com/dwayne/playwhe/tarball/master | tar -xz --directory=git-playground --strip-components=1

$ cd git-playground

# Configure the Git user's name and email
$ sed -i "s/Dwayne R\. Crooks/John Doe/" install-git
$ sed -i "s/me@dwaynecrooks\.com/john\.doe@example\.com/" install-git

# Bring up the VM and log in
$ vagrant up
$ vagrant ssh

# Now you're in you can play around with Git
$ mkdir example && cd example
$ echo 'Hello, world!' > hello
$ git init
$ git add .
$ git ci -m "Initial commit"
$ git hist
```

# Learn

**Free**

- [Atlassian Git Tutorial](https://www.atlassian.com/git/tutorials/)
- [Pro Git](http://git-scm.com/book)
- [Git Magic](http://www-cs-students.stanford.edu/~blynn/gitmagic/)

**Paid**

- [Goal-Oriented Git](https://gumroad.com/l/goal-oriented-git)
- [Mastering Git](https://upcase.com/mastering-git)
- [Git on Code School](https://www.codeschool.com/paths/git)
