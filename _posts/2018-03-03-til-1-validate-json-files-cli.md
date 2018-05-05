---
layout: article
title:  "Today I Learned #1 - Validate JSON Files using CLI"
date:   2018-03-03 16:38:47 +0800
updated_date:   2018-03-03 16:38:47 +0800
group: "blog"
comments: true
---
Install `jsonlint`
<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=install-jsonlint.sh" type="text/javascript"></script>

Navigate to the directory and validate all `.json` files in that directory.
<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=use-jsonlint.sh" type="text/javascript"></script>

This will output the syntax that is causing an error in my case it was `<<<<< HEAD` that I missed from rebasing.

Next thing we do is find the file.

Install `ack-grep`
<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=install-ack-grep.sh" type="text/javascript"></script>
Then run
<script src="https://gist.github.com/iamdevlinph/e01b549ed51d7334f03483ecae1149e9.js?file=use-ack-grep.sh" type="text/javascript"></script>

This will output the directory of the culprit file.

## Things that can be improved on
<hr class='divider--fade' />

Print out the direct and the file name in the `jsonlint` script. I will update the script if I will be able to find out how or if someone can point it out.

## Sources
<hr class='divider--fade' />

- [Detect invalid JSON files in directory tree](https://superuser.com/a/699897/678407)
- [how to find a word in text files from a directory](https://askubuntu.com/a/462279/634714)
