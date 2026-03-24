# StephenBeban.github.io

The code for https://stephenbeban.com. Built with [Jeykll](https://jekyllrb.com/) using the [AcademicPages](https://github.com/academicpages/academicpages.github.io) template.

# Configuration

* **Page content** - (text etc) is stored in the [`_pages`](./_pages) folder
    * These are files written in [Markdown](https://www.markdownguide.org/basic-syntax/). They can be edited in the Github UI or with a simple text editor like Notepad
* **Files** (CSVs, PDFs, Excel files, etc) are stored in the [`files`](/files) folder

More info at https://academicpages.github.io/

# Making changes

There are two ways to make changes to the content of the website:

1. Making changes <u>within the GitHub UI</u> 
    - e.g. Go to the [about.md](https://github.com/StephenBeban/StephenBeban.github.io/blob/main/_pages/about.md) file, click the pencil ✏️ icon, make your changes, save the changes
2. Making your changes locally
    - More on this in the section below

## Running locally

When working on the website, it can be useful to preview changes locally before pushing them to GitHub. To do this you will need to perform the following steps.

Have this repository downloaded to a folder on your local computer.


Have the Ruby programming language installed. For Windows, the installer can be found on this page: https://rubyinstaller.org/downloads/ . Version **3.3.10** works well. Once you have downloaded this installer, run it and proceed through the installation wizard to install Ruby.

When the installer is finished, verify you have Ruby installed by opening a **Terminal** and typing:

```
ruby -v
```

This should give output something like `ruby 3.3.10 (2025-10-23 revision 343ea05002)`, confirming Ruby installed successfully.

After this, you want to install the software packages that will be used to run the website (e.g. the Jekyll package). To do this, open a new **Terminal** inside the `StephenBeban.github.io` folder by right-clicking inside the folder and clicking **Open in Terminal**.

Then inside the folder, type:

```
rake install
```

You should see output something like this:

```
Installing gem dependencies...
bundle install
[DEPRECATED] Platform :mingw, :mswin, :x64_mingw will be removed in the future. Please use platform :windows instead.
Bundle complete! 9 Gemfile dependencies, 98 gems now installed.
Use `bundle info [gemname]` to see where a bundled gem is installed.
```

Finally, to actually run the website on your local machine, run the command below and go to http://localhost:4000 - where you will see the local version of your website.

```
rake serve
```
