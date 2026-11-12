# Quickstart for GitHub Codespaces

Get started with GitHub Codespaces quickly.

## Introduction

In this guide, you'll create a codespace from a template repository and explore some of the essential features available to you within the codespace. You'll work in the browser version of Visual Studio Code, which is initially the default editor for GitHub Codespaces. After trying out this quickstart you can use Codespaces in other editors, and you can change the default editor. Links are provided at the end of this guide.

From this quickstart, you'll learn how to create a codespace, connect to a forwarded port to view your running application, publish your codespace to a new repository, and personalize your setup with extensions.

For more information on exactly how GitHub Codespaces works, see the companion guide [Deep dive into GitHub Codespaces](/en/codespaces/about-codespaces/deep-dive).

## Creating your codespace

1. Navigate to the [github/haikus-for-codespaces](https://github.com/github/haikus-for-codespaces) template repository.
2. Click **Use this template**, then click **Open in a codespace**.

   ![Screenshot of the "Use this template" button and the dropdown menu expanded to show the "Open in a codespace" option.](/assets/images/help/repository/use-this-template-button.png)

## Running the application

Once your codespace is created, the template repository will be automatically cloned into it. Now you can run the application and launch it in a browser.

1. When the terminal becomes available, enter the command `npm run dev`. This example uses a Node.js project, and this command runs the script labeled "dev" in the `package.json` file, which starts up the web application defined in the sample repository.

   ![Screenshot of the Terminal in VS Code with the "npm run dev" command entered.](/assets/images/help/codespaces/codespaces-npm-run-dev.png)

   If you're following along with a different application type, enter the corresponding start command for that project.

2. When your application starts, the codespace recognizes the port the application is running on and displays a pop-up message to let you know that the port has been forwarded.

   ![Screenshot of the pop-up message: "Your application running on port 3000 is available." Below this is a green button, labeled "Open in Browser."](/assets/images/help/codespaces/quickstart-port-toast.png)

3. Click **Open in Browser** to view your running application in a new tab.

## Edit the application and view changes

1. Switch back to your codespace and open the `haikus.json` file by clicking it in the Explorer.

2. Edit the `text` field of the first haiku to personalize the application with your own haiku.

3. Go back to the running application tab in your browser and refresh to see your changes.

   <svg version="1.1" width="16" height="16" viewBox="0 0 16 16" class="octicon octicon-light-bulb" aria-label="light-bulb" role="img"><path d="M8 1.5c-2.363 0-4 1.69-4 3.75 0 .984.424 1.625.984 2.304l.214.253c.223.264.47.556.673.848.284.411.537.896.621 1.49a.75.75 0 0 1-1.484.211c-.04-.282-.163-.547-.37-.847a8.456 8.456 0 0 0-.542-.68c-.084-.1-.173-.205-.268-.32C3.201 7.75 2.5 6.766 2.5 5.25 2.5 2.31 4.863 0 8 0s5.5 2.31 5.5 5.25c0 1.516-.701 2.5-1.328 3.259-.095.115-.184.22-.268.319-.207.245-.383.453-.541.681-.208.3-.33.565-.37.847a.751.751 0 0 1-1.485-.212c.084-.593.337-1.078.621-1.489.203-.292.45-.584.673-.848.075-.088.147-.173.213-.253.561-.679.985-1.32.985-2.304 0-2.06-1.637-3.75-4-3.75ZM5.75 12h4.5a.75.75 0 0 1 0 1.5h-4.5a.75.75 0 0 1 0-1.5ZM6 15.25a.75.75 0 0 1 .75-.75h2.5a.75.75 0 0 1 0 1.5h-2.5a.75.75 0 0 1-.75-.75Z"></path></svg> If you've closed the browser tab, click the Ports tab in VS Code, hover over the **Local Address** value for the running port, and click the **Open in Browser** icon.

   ![Screenshot of the "Ports" panel. The "Ports" tab and a globe icon, which opens the forwarded port in a browser, are highlighted with orange outlines.](/assets/images/help/codespaces/quickstart-forward-port.png)

## Committing and pushing your changes

Now that you've made a few changes, you can use the integrated terminal or the source view to publish your work to a new repository.

1. In the Activity Bar, click the **Source Control** view.

   ![Screenshot of the VS Code Activity Bar with the source control button highlighted with an orange outline.](/assets/images/help/codespaces/source-control-activity-bar-button.png)

2. To stage your changes, click <svg version="1.1" width="16" height="16" viewBox="0 0 16 16" class="octicon octicon-plus" aria-label="Stage Changes" role="img"><path d="M7.75 2a.75.75 0 0 1 .75.75V7h4.25a.75.75 0 0 1 0 1.5H8.5v4.25a.75.75 0 0 1-1.5 0V8.5H2.75a.75.75 0 0 1 0-1.5H7V2.75A.75.75 0 0 1 7.75 2Z"></path></svg> next to the `haikus.json` file, or next to **Changes** if you've changed multiple files and you want to stage them all.

   ![Screenshot of the "Source control" side bar with the staging button (a plus sign), to the right of "Changes," highlighted with a dark orange outline.](/assets/images/help/codespaces/codespaces-commit-stage.png)

3. To commit your staged changes, type a commit message describing the change you've made, then click **Commit**.

   ![Screenshot of the "Source control" side bar. The commit message, "Change haiku text and styles," and the "Commit" button are outlined in orange.](/assets/images/help/codespaces/vscode-commit-button.png)

4. Click **Publish Branch**.

   ![Screenshot of the "Source control" side bar showing the "Publish Branch" button.](/assets/images/help/codespaces/vscode-publish-branch-button.png)

5. In the "Repository Name" dropdown, type a name for your new repository, then select **Publish to GitHub private repository** or **Publish to GitHub public repository**.

   ![Screenshot of the repository name dropdown in VS Code. Two options are shown, for publishing to a private or a public repository.](/assets/images/help/codespaces/choose-new-repository.png)

   The owner of the new repository will be the GitHub account with which you created the codespace.

6. In the pop-up that appears in the lower right corner of the editor, click **Open on GitHub** to view the new repository on GitHub. In the new repository, view the `haikus.json` file and check that the change you made in your codespace has been successfully pushed to the repository.

   ![Screenshot of a confirmation message for a successfully published repository, showing the "Open on GitHub" button.](/assets/images/help/codespaces/open-on-github.png)

## Personalizing with an extension

When you connect to a codespace using the browser, or the Visual Studio Code desktop application, you can access the Visual Studio Code Marketplace directly from the editor. For this example, you'll install a VS Code extension that alters the theme, but you can install any extension that's useful for your workflow.

1. In the Activity Bar, click the Extensions icon.

   ![Screenshot of the Activity Bar. The Extensions icon is highlighted with an orange outline.](/assets/images/help/codespaces/extensions-activity-bar-icon.png)

2. In the search bar, type `fairyfloss` and click **Install**.

   ![Screenshot of "Extensions: Marketplace". The search box shows "fairyfloss." The results show the "fairyfloss" extension with an "Install" button.](/assets/images/help/codespaces/add-extension.png)

3. Select the `fairyfloss` theme by selecting it from the list.

   ![Screenshot of the "Select Color Theme" dropdown, with the "fairyfloss" theme selected.](/assets/images/help/codespaces/fairyfloss.png)

### About Settings Sync

You can enable Settings Sync to sync extensions and other settings across devices and instances of VS Code. Your synced settings are cached in the cloud. If Settings Sync is turned on in a codespace, any updates you make to your settings in the codespace are pushed to the cloud, and any updates you push to the cloud from elsewhere are pulled into your codespace. For more information, see [Personalizing GitHub Codespaces for your account](/en/codespaces/setting-your-user-preferences/personalizing-github-codespaces-for-your-account#settings-sync).

## Next steps

You've successfully created, personalized, and run your first application within a codespace but there's so much more to explore! Here are some helpful resources for taking your next steps with GitHub Codespaces.

* [Deep dive into GitHub Codespaces](/en/codespaces/about-codespaces/deep-dive): This quickstart presented some of the features of GitHub Codespaces. The deep dive looks at these areas from a technical standpoint.
* [Adding a dev container configuration to your repository](/en/codespaces/setting-up-your-project-for-codespaces/adding-a-dev-container-configuration): These guides provide information on setting up your repository to use GitHub Codespaces with specific languages.
* [Introduction to dev containers](/en/codespaces/setting-up-your-project-for-codespaces/adding-a-dev-container-configuration/introduction-to-dev-containers): This guide provides details on creating a custom configuration for Codespaces for your project.

## Further reading

* [Enabling or disabling GitHub Codespaces for your organization](/en/codespaces/managing-codespaces-for-your-organization/enabling-or-disabling-github-codespaces-for-your-organization)
* [Using GitHub Codespaces in Visual Studio Code](/en/codespaces/developing-in-a-codespace/using-github-codespaces-in-visual-studio-code)
* [Using GitHub Codespaces with GitHub CLI](/en/codespaces/developing-in-a-codespace/using-github-codespaces-with-github-cli)
* [Setting your default editor for GitHub Codespaces](/en/codespaces/setting-your-user-preferences/setting-your-default-editor-for-github-codespaces)
* [Managing the cost of GitHub Codespaces in your organization](/en/codespaces/managing-codespaces-for-your-organization/managing-the-cost-of-github-codespaces-in-your-organization)

This is Python version 3.14.2
=============================

.. image:: https://github.com/python/cpython/actions/workflows/build.yml/badge.svg?branch=main&event=push
   :alt: CPython build status on GitHub Actions
   :target: https://github.com/python/cpython/actions

.. image:: https://dev.azure.com/python/cpython/_apis/build/status/Azure%20Pipelines%20CI?branchName=main
   :alt: CPython build status on Azure DevOps
   :target: https://dev.azure.com/python/cpython/_build/latest?definitionId=4&branchName=main

.. image:: https://img.shields.io/badge/discourse-join_chat-brightgreen.svg
   :alt: Python Discourse chat
   :target: https://discuss.python.org/


Copyright © 2001 Python Software Foundation.  All rights reserved.

See the end of this file for further copyright and license information.

.. contents::

General Information
-------------------

- Website: https://www.python.org
- Source code: https://github.com/python/cpython
- Issue tracker: https://github.com/python/cpython/issues
- Documentation: https://docs.python.org
- Developer's Guide: https://devguide.python.org/

Contributing to CPython
-----------------------

For more complete instructions on contributing to CPython development,
see the `Developer Guide`_.

.. _Developer Guide: https://devguide.python.org/

Using Python
------------

Installable Python kits, and information about using Python, are available at
`python.org`_.

.. _python.org: https://www.python.org/

Build Instructions
------------------

On Unix, Linux, BSD, macOS, and Cygwin::

    ./configure
    make
    make test
    sudo make install

This will install Python as ``python3``.

You can pass many options to the configure script; run ``./configure --help``
to find out more.  On macOS case-insensitive file systems and on Cygwin,
the executable is called ``python.exe``; elsewhere it's just ``python``.

Building a complete Python installation requires the use of various
additional third-party libraries, depending on your build platform and
configure options.  Not all standard library modules are buildable or
usable on all platforms.  Refer to the
`Install dependencies <https://devguide.python.org/getting-started/setup-building.html#build-dependencies>`_
section of the `Developer Guide`_ for current detailed information on
dependencies for various Linux distributions and macOS.

On macOS, there are additional configure and build options related
to macOS framework and universal builds.  Refer to `Mac/README.rst
<https://github.com/python/cpython/blob/main/Mac/README.rst>`_.

On Windows, see `PCbuild/readme.txt
<https://github.com/python/cpython/blob/main/PCbuild/readme.txt>`_.

To build Windows installer, see `Tools/msi/README.txt
<https://github.com/python/cpython/blob/main/Tools/msi/README.txt>`_.

If you wish, you can create a subdirectory and invoke configure from there.
For example::

    mkdir debug
    cd debug
    ../configure --with-pydebug
    make
    make test

(This will fail if you *also* built at the top-level directory.  You should do
a ``make clean`` at the top-level first.)

To get an optimized build of Python, ``configure --enable-optimizations``
before you run ``make``.  This sets the default make targets up to enable
Profile Guided Optimization (PGO) and may be used to auto-enable Link Time
Optimization (LTO) on some platforms.  For more details, see the sections
below.

Profile Guided Optimization
^^^^^^^^^^^^^^^^^^^^^^^^^^^

PGO takes advantage of recent versions of the GCC or Clang compilers.  If used,
either via ``configure --enable-optimizations`` or by manually running
``make profile-opt`` regardless of configure flags, the optimized build
process will perform the following steps:

The entire Python directory is cleaned of temporary files that may have
resulted from a previous compilation.

An instrumented version of the interpreter is built, using suitable compiler
flags for each flavor. Note that this is just an intermediary step.  The
binary resulting from this step is not good for real-life workloads as it has
profiling instructions embedded inside.

After the instrumented interpreter is built, the Makefile will run a training
workload.  This is necessary in order to profile the interpreter's execution.
Note also that any output, both stdout and stderr, that may appear at this step
is suppressed.

The final step is to build the actual interpreter, using the information
collected from the instrumented one.  The end result will be a Python binary
that is optimized; suitable for distribution or production installation.


Link Time Optimization
^^^^^^^^^^^^^^^^^^^^^^

Enabled via configure's ``--with-lto`` flag.  LTO takes advantage of the
ability of recent compiler toolchains to optimize across the otherwise
arbitrary ``.o`` file boundary when building final executables or shared
libraries for additional performance gains.


What's New
----------

We have a comprehensive overview of the changes in the `What's New in Python
3.14 <https://docs.python.org/3.14/whatsnew/3.14.html>`_ document.  For a more
detailed change log, read `Misc/NEWS
<https://github.com/python/cpython/tree/main/Misc/NEWS.d>`_, but a full
accounting of changes can only be gleaned from the `commit history
<https://github.com/python/cpython/commits/main>`_.

If you want to install multiple versions of Python, see the section below
entitled "Installing multiple versions".


Documentation
-------------

`Documentation for Python 3.14 <https://docs.python.org/3.14/>`_ is online,
updated daily.

It can also be downloaded in many formats for faster access.  The documentation
is downloadable in HTML, EPUB, and reStructuredText formats; the latter version
is primarily for documentation authors, translators, and people with special
formatting requirements.

For information about building Python's documentation, refer to `Doc/README.rst
<https://github.com/python/cpython/blob/main/Doc/README.rst>`_.


Testing
-------

To test the interpreter, type ``make test`` in the top-level directory.  The
test set produces some output.  You can generally ignore the messages about
skipped tests due to optional features which can't be imported.  If a message
is printed about a failed test or a traceback or core dump is produced,
something is wrong.

By default, tests are prevented from overusing resources like disk space and
memory.  To enable these tests, run ``make buildbottest``.

If any tests fail, you can re-run the failing test(s) in verbose mode.  For
example, if ``test_os`` and ``test_gdb`` failed, you can run::

    make test TESTOPTS="-v test_os test_gdb"

If the failure persists and appears to be a problem with Python rather than
your environment, you can `file a bug report
<https://github.com/python/cpython/issues>`_ and include relevant output from
that command to show the issue.

See `Running & Writing Tests <https://devguide.python.org/testing/run-write-tests.html>`_
for more on running tests.

Installing multiple versions
----------------------------

On Unix and Mac systems if you intend to install multiple versions of Python
using the same installation prefix (``--prefix`` argument to the configure
script) you must take care that your primary python executable is not
overwritten by the installation of a different version.  All files and
directories installed using ``make altinstall`` contain the major and minor
version and can thus live side-by-side.  ``make install`` also creates
``${prefix}/bin/python3`` which refers to ``${prefix}/bin/python3.X``.  If you
intend to install multiple versions using the same prefix you must decide which
version (if any) is your "primary" version.  Install that version using
``make install``.  Install all other versions using ``make altinstall``.

For example, if you want to install Python 2.7, 3.6, and 3.14 with 3.14 being the
primary version, you would execute ``make install`` in your 3.14 build directory
and ``make altinstall`` in the others.


Release Schedule
----------------

See `PEP 745 <https://peps.python.org/pep-0745/>`__ for Python 3.14 release details.


Copyright and License Information
---------------------------------


Copyright © 2001 Python Software Foundation.  All rights reserved.

Copyright © 2000 BeOpen.com.  All rights reserved.

Copyright © 1995-2001 Corporation for National Research Initiatives.  All
rights reserved.

Copyright © 1991-1995 Stichting Mathematisch Centrum.  All rights reserved.

See the `LICENSE <https://github.com/python/cpython/blob/main/LICENSE>`_ for
information on the history of this software, terms & conditions for usage, and a
DISCLAIMER OF ALL WARRANTIES.

This Python distribution contains *no* GNU General Public License (GPL) code,
so it may be used in proprietary projects.  There are interfaces to some GNU
code but these are entirely optional.

All trademarks referenced herein are property of their respective holders.
