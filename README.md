# Git Playground

Play with the latest [Git][git] in a [virtual machine](https://www.virtualbox.org/).

# Usage

```sh
# If you have Git installed then
$ git clone git@github.com:dwayne/git-playground.git
# Otherwise
$ mkdir git-playground && curl -L https://github.com/dwayne/git-playground/tarball/master | tar -xz --directory=git-playground --strip-components=1

$ cd git-playground

# Configure the Git user's name and email
$ sed -i "s/Dwayne Crooks/John Doe/" install-git
$ sed -i "s/me@dwaynecrooks\.com/john\.doe@example\.com/" install-git

# Bring up the VM and log in
$ vagrant up
$ vagrant ssh

# Now you're in you can play around with Git
$ mkdir example && cd example
$ echo 'Hello, world!' > hello.txt
$ git init
$ git add hello.txt
$ git ci -m "Initial commit"
$ git hist
```

# Learn

**Free**

- [Pro Git](http://git-scm.com/book)
- [Atlassian Git Tutorial](https://www.atlassian.com/git/tutorials/)
- [Git Magic](http://www-cs-students.stanford.edu/~blynn/gitmagic/)

**Paid**

- [Git on Code School](https://www.codeschool.com/learn/git)
- [Mastering Git](https://upcase.com/mastering-git)
- [Goal-Oriented Git](https://gumroad.com/l/goal-oriented-git)

[git]: https://git-scm.com/
