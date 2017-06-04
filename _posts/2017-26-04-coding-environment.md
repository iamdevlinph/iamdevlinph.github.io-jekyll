---
layout: article
title:  "Coding Environment"
date:   2017-06-04 15:46:41 +0800
group: "articles"
---
I've been developing using JavaScript for well over a year now. My coding environment is pretty normal. I have two environments: at the office, and at home.

At the **office**:
<ul class="article_list">
    <li><a href="https://code.visualstudio.com/" target="_blank">Visual Studio Code</a></li>
    <li>Ubuntu 17.04</li>
</ul>

and at **home**:
<ul class="article_list">
    <li><a href="https://code.visualstudio.com/" target="_blank">Visual Studio Code</a></li>
    <li>Windows 10 Version 1703 (Insider Preview)</li>
</ul>

VS Code is also the common denominator between the two, right? So let's talk about it first.

Here's what I love about this editor:
<ul class="article_list">
    <li><a href="https://code.visualstudio.com/docs/editor/versioncontrol" target="blank">Integrated GIT</a></li>
    <li><a href="https://code.visualstudio.com/docs/editor/integrated-terminal" target="_blank">Integrated Terminal</a></li>
</ul>

### Integrated GIT
---
This really makes development easier. This feature makes it easy to track changes in a project.

You can go to the GIT Panel by pressing `Ctrl+Shift+G`. I only have Windows, and the shortcut in Ubuntu is just the same, so yeah.

Here's the integrated GIT in action. In a basic way, anyway.

![alt text]({{ site.url }}/assets/integrated-git/01-integrated-git-min.png "01 Integrated GIT")<br/>
`A` **Reset** - Discards all unstaged stages in a file. Clicking this will show a prompt.<br/>
`B` **Add** - Works just like a `git add <filename>`, adds the file to staging.<br/>
`C` **GIT** Badge - Shows the number of changes done in the current project. As you can see, I have 2 changes.

![alt text]({{ site.url }}/assets/integrated-git/02-integrated-git-min.png "02 Integrated GIT")<br/>
`D` **Added** - This green line indicator means that this line is an added line.

![alt text]({{ site.url }}/assets/integrated-git/03-integrated-git-min.png "03 Integrated GIT")<br/>
`E` **Modified** - This blue line indicator means that a modification has been done on this line.

![alt text]({{ site.url }}/assets/integrated-git/04-integrated-git-min.png "04 Integrated GIT")<br/>
`F` **Deleted** - This red line indicator means that a deletion as been done on this line.

There was also a feature to `add specific line(s) to staging` but they somehow removed it.

### Integrated Terminal
---
Well, I've stopped using this since I just do the all the other `GIT` stuff, aside from `git add`, in the Terminal.

### Windows or Linux?
---
From what I observe, belows is my comparison.
<table class="standard side-by-side">
    <tr>
        <th colspan="2">Windows</th>
    </tr>
    <tr>
        <th>Pros</th>
        <th>Cons</th>
    </tr>
    <tr>
        <!-- Windows Pros -->
        <td>
            <ul class="pros_list">
                <li>Can game for a break</li>
                <li>Has Bash for Windows now</li>
            </ul>
        </td>
        <!-- Windows Cons -->
        <td>
            <ul class="cons_list">
                <li>Have some issues with NPM</li>
                <li>Terminal cannot be tabbed, needs emulator to achieve</li>
            </ul>
        </td>
    </tr>
</table>

<table class="standard side-by-side">
    <tr>
        <th colspan="2">Ubuntu</th>
    </tr>
    <tr>
        <th>Pros</th>
        <th>Cons</th>
    </tr>
    <tr>
        <!-- Ubuntu Pros -->
        <td>
            <ul class="pros_list">
                <li>No issues with NPM so far</li>
            </ul>
        </td>
        <!-- Ubuntu Cons -->
        <td>
            <ul class="cons_list">
                <li>Very resource hogger</li>
                <li>Freezes when runs out of memory</li>
            </ul>
        </td>
    </tr>
</table>

Not really much reason to prefer one  over the other. I've been using both and I haven't experienced any issue that makes me drop everything and switch to the other.
