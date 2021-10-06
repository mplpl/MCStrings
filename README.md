# MCStrings

This repo contains strings and other localizable content (like HTML pages with the help) of MaxCommander project. Currently, the files come from version 2.1.

## Adding a new translation

If you want to translate to a new language, create a top-level directory indicating that locale (for instance 'fr' for French) and copy there all the files from the 'to_translate' folder. Next, translate all these files and commit/push them back to this repo. 

More detailed instruction (using a new French translation as an example:

1. Make sure you have an account on github.com and a 'git' command installed on your workstation
2. On your workstation, call the following commands:

```
git clone https://github.com/mplpl/MCStrings
cd MCStrings
git checkout -b new_fr_translation
cp -rf to_translate fr
git add fr
```

Now you should have a new branch with the name 'new_fr_translation' where you have the 'fr' folder copied from 'to_translate'

3. Translate the content of the 'fr' folder
4. Commit changes to your local branch:

```
git commit -a -m "new French translation"
```

5. Push the branch to github.com:

```
git push --set-upstream origin new_fr_translation
```

6. Go to 'https://github.com/mplpl/MCStrings' and open a pull request from your branch to 'main'
- on the page, click 'Pull Requests' tab
- select 'main' as 'base' and your branch (here 'new_fr_translation') as 'compare'
- click 'Create pull request' button

Next, your pull request will be reviewed and merged by the project maintainers.

## License and rights

Please note, that all the files in this repo, including the files that you add, are covered by MIT license which allows to use them in commercial products without any liability or payment to whoever added or modified them in this repo.
