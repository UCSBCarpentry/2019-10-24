# workshop-template

Customizing is at this point from template Readme.md:


## Customizing Your Website



3.  Edit the header of `index.md` to customize the list of instructors,
    workshop venue, etc. 
    You can do this in the browser by clicking on it in the file view on GitHub
    and then selecting the pencil icon in the menu bar:

    ![](fig/edit-index-file-menu-bar.png?raw=true)
    
    Editing hints are embedded in `index.md`,
    and full instructions are in [the customization instructions][customization].

STUCK HERE! Eventbrite not showing up.  Some stuff below has already been completed.
AMY form is already submitted.



4.  Edit `_config.yml` to customize certain site-wide variables, such as: `carpentry` (to tell us which carpentry workshop this is), `title` (overall title for all pages), `workshop_repo` (the URL of the workshop repository on GitHub) and `workshop_site` (the repository's GitHub Pages URL).

    Editing hints are embedded in `_config.yml`,
    and full instructions are in [the customization instructions][customization].
    
5. Edit the `schedule.html` file to edit the schedule for your upcoming workshop. This file is located in the `_includes` directory, make sure to choose the one from the appropriate `dc` (Data Carpentry workshop), `lc` (Library Carpentry), or `swc` (Software Carpentry) subdirectory.


7.  When you are done editing,
    go to the GitHub Pages URL for your workshop and preview your changes.
    In the example above, this is `https://gvwilson.github.io/2016-12-01-miskatonic`.
    The finished page should look [something like this](fig/completed-page.png?raw=true).

8.  Optional: you can now change the README.md file in your website's repository, which contains these instructions, so that it contains a short description of your workshop and a link to the workshop website.

9.  Optional: Add a link to your workshop website on the repository main page in the description/website section (look for the `Edit` button on the right to add).  

**Note:**
please do all of your work in your repository's `gh-pages` branch,
since [GitHub automatically publishes that as a website][github-project-pages].

**Note:**
this template includes some files and directories that most workshops do not need,
but which provide a standard place to put extra content if desired.
See the [design notes][design] for more information about these.

Further instructions are available in [the customization instructions][customization].
This [FAQ][faq] includes a few extra tips (additions are always welcome)
and these notes on [the background and design][design] of this template may help as well.

## (Optional) Linking to Your Page

At the top of your repository on GitHub you'll see

~~~
No description, website, or topics provided. — Edit
~~~

Click 'Edit' and add:

1.  A very brief description of your workshop in the "Description" box (e.g., "Miskatonic University workshop, Dec. 2016")

2.  The URL for your workshop in the "Website" box (e.g., `https://gvwilson.github.io/2016-12-01-miskatonic`)

This will help people find your website if they come to your repository's home page.

## Creating Extra Pages

In rare cases,
you may want to add extra pages to your workshop website.
You can do this by putting either Markdown or HTML pages in the website's root directory
and styling them according to the instructions give in
[the lesson template][lesson-example].
If you do this,
you *must* also edit `_config.yml` to set these three values:

1.  `carpentry` is either "dc" (for Data Carpentry), "swc" (for Software Carpentry),
    or "lc" (for Library Carpentry). This determines which logos are loaded.

2.  `title` is the title of your workshop (typically the venue and date).

3.  `email` is the contact email address for your workshop,
    e.g., `gvwilson@miskatonic.edu`.

Note: `carpentry` and `email` duplicate information that's in `index.md`,
but there is no way to avoid this
without requiring people to edit both files in the usual case
where no extra pages are created.



## Setting Up a Separate Repository for Learners

If you are teaching Git,
you should create a separate repository for learners to use in that lesson.
You should not have them use the workshop website repository because:

*   your workshop website repository contains many files
    that most learners don't need to see during the lesson,
    and

*   you probably don't want to accidentally merge
    a damaging pull request from a novice Git user
    into your workshop's website while you are using it to teach.

You can call this repository whatever you like,
and add whatever content you need to it.


