# Put this site live at 7sanjayg.github.io

Your username `7SanjayG` is confirmed, and nothing is published there yet.

Naming the repo `7SanjayG.github.io` is the fastest route, because GitHub Pages
serves that one repo automatically from the default branch. There is no
Settings step and no build to configure.

**Your URL will be:** `https://7sanjayg.github.io`

GitHub lower-cases the subdomain, so that is the canonical form even though
your username has capitals. Either spelling resolves.

---

## Step 1 — create the repo

Go to https://github.com/new and set:

| Field | Value |
|---|---|
| Repository name | `7SanjayG.github.io` |
| Visibility | **Public** (required for free GitHub Pages) |
| Initialise with README | **leave unticked** |

Create it, then close the page.

## Step 2 — push

Run this from `E:\JAI\submission\site`:

```bash
git init -b main && git add -A && git commit -m "JAI landing page" && git remote add origin https://github.com/7SanjayG/7SanjayG.github.io.git && git push -u origin main
```

If git asks for credentials, use your GitHub username and a personal access
token as the password. Tokens are created at
https://github.com/settings/tokens, and the `repo` scope is enough.

## Step 3 — check it

The first build takes about a minute. Then open

```
https://7sanjayg.github.io
```

in a **private browser window**, signed out. That is the same way an evaluator
will open it, and the competition disqualifies a link they cannot reach.

---

## If you would rather keep the root clean

Name the repo `jai` instead, push the same way, then go to **Settings → Pages**
and set Source to `main` with folder `/ (root)`. The URL becomes
`https://7sanjayg.github.io/jai/`. This takes one extra step, which is the only
reason it is the second choice.

## What is on the page

One screen of substance, in the deck's design language: the problem, the five
gate checks, the three headline numbers with their scope stated, and the
hardware JAI has designed. `.nojekyll` is included so GitHub serves the files
as-is.

Next session we can build this out properly: the part gallery with the renders,
the gate report rendered as a live table, and downloadable STEP files.

Note that the repo and the page are public, which is what free GitHub Pages
requires. Nothing on the page is sensitive, and every number on it carries its
scope.
