# Collaboration Skills

## Writing comments

Facilitating collaboration is one of the things GitHub is designed to do.
That means that there are many places for discussion:
pull requests, issues, discussion boards, comments belows Gists, etc.
There are several things that you can do when writing these comments,
to make them more readable and informative.

### Use Markdown

You can write your comments with Markdown syntax, just like you may already
be doing in your `README.md` files.
Some Markdown syntax that can be particularly useful for comments on GitHub:

#### blockquotes

Use these to quote some/all of a previous message in the thread

```
> written with a preceding greater-than symbol, like this
>> or two, for a quote-within-a-quote
```


#### Code blocks

Write code inline with `single backticks` and blocks with triple backticks:

```
import pandas as pd

skills_data = pd.read_csv("data/github-skills.csv", index_col=0)
skills_data.head
```

and place the name of the language after the opening three backticks,
to enable syntax highlighting for that code block:

```Python
import pandas as pd

skills_data = pd.read_csv("data/github-skills.csv", index_col=0)
skills_data.head
```

### Refer to other things on GitHub

#### Issues and pull requests

To refer to an issue/pull request (PR) within the same repository,
type the `#` symbol followed by the number of that issue/PR, e.g. #1.

If refering to an issue/PR on another repository, add the namespace and name
of the repository before the `#`, e.g.

> carpentries-incubator/jekyll-pages-novice#251

When opening a pull request to fix an open issue on the repository,
you can type

> Fixes #1

in the PR description and, if/when the PR is merged, the corresponding issue will
be closed automatically.
[As well as _fixes_, you can use, _resolves_, and _closes_](https://docs.github.com/en/github/writing-on-github/working-with-advanced-formatting/using-keywords-in-issues-and-pull-requests).

#### Commits

You may want to refer to a particular commit in the version history of the project,
e.g. to identify exactly when a particular change was made/bug was introduced.
You can do this by copying and pasting the _hash_ of the commit
(that long string of characters associated with each commit in Git). E.g.

> c15c9ab8d418b4c675fceb50722478925fed2c34

You don't even need to copy the whole hash:
the first seven characters is sufficient for GitHub to identify the commit.

### Reviewing a pull request

To review a PR, open the "diff" view (click the _Files changed_ tab of the PR page).

#### Commenting on specific lines/changes

If you want to talk about a specific change within a larger pull request,
hover your mouse over the (first) line you want to comment on.
You should see a blue `+` symbol appear to the left of that line.

Click that plus, to comment on the single line, or click and drag down to the last line
where the changes of interest end.
You should get a new dialogue box into which you can write your comment.
When submitting the comment,
you can choose to add it as a single comment,
or queue it up in a batch of comments to be published when you finish your review.

**Practice by adding a comment on one of the lines in this file in this pull request**.

#### Suggesting changes

When commenting on a line, you might want to suggest the exact change you would
like to see made to the PR. (This can be really helpful for wording and typo fixes.)
You can do this by clicking the little file-with-a-plus-minus-symbol ± icon
above the comment box.

Clicking that icon will populate the comment box with the content of the line(s)
you selected in the PR, surrounded by backticks. If you modify this content in your comment, to make
the change you want to suggest, you can then submit this comment as a suggestion
on the PR.
(Add any explanation to give context to the suggested change beneath the closing backticks.)

Suggest changes can be merged directly by the PR author, and both they and you will be listed as co-authors on that commit.

**Practice by making a suggestion to fix a typo in the block of text below.**
([Credit to Julia Donaldson for the source text](https://www.juliadonaldson.co.uk/books/picture-books/the-snail-and-the-whale/).)

> This is the tale fo a tinyy snail
> And a ggreat biig, grey-blue humpback whale.
> This is a rock as black as soot
> And this si a snnail withan itchy foot.
> The sea snail slithered alll over the rock
> Andd gazed at the sea and the ships in the dock.
> And as she gazed,, she sniffed and sighed,
> "The se is deep and the world is wide."
> "How Ilong to sail," said the tiny snail.

#### Finish your review

When you are done commenting/suggesting,
click the _Review changes_ or _Finish your review_ button
(depending on whether you have any comments/suggestion pending)
near the top-right of the window.

Add some summary comments to accompany your specific remarks and,
if you have the appropriate privileges on the repository, choose an option:

- _Comment_: do not explicitly approve or ask for changes to the PR, but make a general comment.
- _Approve_: approve the changes as they are currently in the PR.
- _Request changes_: ask the author to make one or more changes before the PR is merged.
