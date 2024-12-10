======================
Publishing HTML Files
======================

This document provides step-by-step instructions for publishing the HTML documentation of your Python project to:

1. ReadTheDocs.org
2. GitHub Pages

Prerequisites
==============

- Generated HTML files from Sphinx (`_build/html` directory).
- A GitHub account.
- ReadTheDocs account (if using ReadTheDocs.org).

Publishing to ReadTheDocs.org
=============================

Step 1: Create a ReadTheDocs Project
------------------------------------

1. Log in to your ReadTheDocs account at https://readthedocs.org/.
2. Click on **+ Import a Project**.
3. Select the **Connect to GitHub** option and authorize ReadTheDocs to access your repositories.
4. Choose your project repository from the list or add a new repository.

Step 2: Configure ReadTheDocs
-----------------------------

1. Navigate to your project's settings in ReadTheDocs.
2. Under the **Admin > Advanced Settings** section, specify the following:
   - **Python configuration file**: `docs/conf.py` (or the location of your `conf.py` file).
   - **Documentation type**: Sphinx HTML.
   - **Requirements file**: `requirements.txt` (if you have additional Python dependencies).
3. Save the changes.

Step 3: Trigger a Build
-----------------------

1. Trigger a build by clicking the **Build Version** button on the project's dashboard.
2. Once the build is complete, your documentation will be live at `<project-name>.readthedocs.io`.

Step 4: Maintain Updates
------------------------

1. Push changes to your GitHub repository.
2. ReadTheDocs automatically rebuilds the documentation on new commits.

Publishing to GitHub Pages
==========================

Step 1: Create a GitHub Repository
-----------------------------------

1. Go to https://github.com/.
2. Click on **+ New Repository**.
3. Name the repository (e.g., `sphinx-dempo-app`).
4. Set the repository as **Public**.
5. Click **Create Repository**.

Step 2: Add HTML Files to the Repository
----------------------------------------

1. Navigate to your project's `_build/html` directory.
2. Copy the entire contents of the `html` directory.
3. Clone the GitHub repository locally:

.. code:: bash

    git clone https://github.com/<username>/project-docs.git

4. Paste the HTML files into the cloned repository.
5. Add, commit, and push the files to GitHub:

Step 3: Enable GitHub Pages
---------------------------

1. Go to your repository on GitHub.
2. Navigate to **Settings > Pages**.
3. Under **Source**, select the `main` branch and `/ (root)` folder.
4. Click **Save**.
5. Your documentation will be live at `https://<username>.github.io/project-docs/`.

Step 4: Maintain Updates
------------------------

1. Update the `_build/html` directory in your local repository.
2. Push changes to GitHub:

.. code:: bash

    git add . git commit -m "Update documentation" git push origin main

Tips for Managing Documentation
===============================

- Always generate updated HTML files using Sphinx before publishing.
- Keep the `conf.py` and `requirements.txt` files updated with any project changes.
- Use meaningful commit messages for documentation updates.

Further Assistance
==================

- ReadTheDocs documentation: https://docs.readthedocs.io/
- GitHub Pages guide: https://docs.github.com/en/pages
