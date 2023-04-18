# **What is Git?**

**Git** is a console tool for tracking and maintaining a history of file changes in your project. Most often it is used for code, but it can be used for other files as well. For example, for pictures - useful for designers.

With **Git** - you can rollback your project to an older version, compare, analyze or merge your changes into a **repository**.

**Repository** refers to the repository of your code and the history of its changes. **Git** works locally and all your repositories are stored in specific folders on your hard drive.

Also, your repositories can be stored on the Internet. Usually three services are used for this:

- [GitHub](https://github.com/)
- [Bitbucket](https://bitbucket.org/)
- [GitLab](https://gitlab.com/)

Each savepoint in your project is named **commit**. Each **commit** has a **hash (unique id)** and a comment. From such **commit**-s a **branch** is built. **Branch** is the history of changes. Each branch has its own name. A repository can contain several branches that are created from or merged into other branches.

# **How Git works**

If you look at the picture, it becomes a little easier with understanding. Each circle is a **commit**. The arrows show the direction from which **commit** the next is made. For example, `C3` is made from `C2`, etc. All these **commit** are in a branch called `main`. This is the master branch, most commonly referred to as `master` . The `main*` rectangle shows which **commit** we are currently in, in other words, a pointer.

![](assets/1.jpeg)

The result is a very simple graph consisting of one branch (main) and four commits. All this can turn into a more complex graph, consisting of several branches that merge into one.

![](assets/bugFix.gif)

# **Initial Git setup**

1. Run installed git bash program (black, scary terminal)
2. Enter the command `git config --global user.name "Firstname Lastname"` and press **Enter**
3. Enter the command `git config --global user.email <email>` and press **Enter**
4. Check if the settings have been applied with the command `git config --list --show-origin`
   If the terminal shows the entered username and email, then everything is OK
   read online for free

# **Basic command line operations (terminal, console)**

Before you start using the git, you need to master the basic commands that are executed in the operating system through the terminal.

**ls**

- The most commonly used command is `ls`
- This command lists the files in the current active directory.
- Show all files, including hidden ones: `ls -a`

**cd**

- By default, the terminal opens in the user's directory, i.e. in the home folder on your computer's hard drive.
- Moving through directories is done with the command `cd “directory name”`
- Move up a directory one level up: `cd ..`
- Move up a directory 2 levels up: `cd ../..`

**mkdir**

- Command to create a directory: `mkdir “directory name”`

**touch**

- Command to create an empty file: `touch “filename”`

**cp**

- Command for copying a file: `cp “name of the copied file” “new name of the copied file”`

**mv**

- Command to rename a file: `mv “file name” “new filename”`

**echo**

- Command to write to file: `echo “Text” > “filename”`

**cat**

- View file contents: `cat “filename”`

**rm**

- Command to delete a file:`rm “filename”`

**rm -R**

- Command to recursively remove (remove all files inside a directory and the directory itself) a directory: `rm -R “directory name”`
