# KLEAR Website

Website code for KLEAR, a research team at Princeton University run by [Karthik Narasimhan](https://www.cs.princeton.edu/~karthikn/) studying natural language processing.

Built on top of [Archie](https://github.com/athul/archie) theme, based on [Hugo](https://gohugo.io/) framework.

## Setup

1. Install Hugo (instructions can be found [here](https://gohugo.io/getting-started/installing/)).
2. Clone this repo
3. Run `hugo server` in your local directory. A website preview should be visible on http://localhost:1313/

### Usage

For below changes, please make sure to run `hugo server` locally and visually confirm that the changes were made successfully.

Then, create a PR. The website czar will double check, then merge the PR if all looks well.

**Add a new person**

1. Open the `config.yml` file
2. Navigate to the `authors` [key](https://github.com/carlosejimenez/lab-website/blob/main/config.yml#L12)
3. Under the `authors` key, add your username (i.e. `carlosej`) as a new key.
4. Add the following as key-value pairs under your username key
   - Required: `name`, `link`, `pic` (see below for extra details)
   - Optional: `github`, `scholar`, `twitter`
5. Add your username to the `people` [list](https://github.com/carlosejimenez/lab-website/blob/main/content/people.md)
6. Launch the website, then check the "People" tab to confirm your profile was added

You may add either a link or a static asset as your `pic`.

- (Recommended) For a static asset...
  - Add your image to the `static/images/people` [folder](https://github.com/carlosejimenez/lab-website/tree/main/static/images/people)
  - Add the name of your image as the field of pic `i.e. pic: jy1682.jpg`
- For a link, paste the link (i.e. `pic: http://...`)

**Add a new post**

**Add a new publication**
