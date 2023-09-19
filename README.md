# git-vimstage

Makes it possible to use `vimdiff` (or [Meld](https://meldmerge.org/), or whatever) instead of `git add -p`/`git add -e` for fine-grained staging.

If file is not staged yet, opens regular `$EDITOR`.

## Usage

```sh
# defaults to vimdiff
git config --add --global vimstage.editor meld
# or, if you want to try another editor
export DEDITOR=meld

git vimstage ./foo
# and see what you did:
git diff --cached ./foo
```
