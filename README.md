# 🤖 KLEAR Website

Website code for KLEAR, a research team at Princeton University run by [Karthik Narasimhan](https://www.cs.princeton.edu/~karthikn/) studying natural language processing.

Built on top of [Archie](https://github.com/athul/archie) theme, based on [Hugo](https://gohugo.io/) framework.

## 🛠️ Setup

1. Install Hugo (instructions can be found [here](https://gohugo.io/getting-started/installing/)).
2. Clone this repo
3. Run `hugo server` in your local directory. A website preview will be visible on http://localhost:1313/

## 🖋️ Usage

For below changes, please make sure to run `hugo server` locally and visually confirm that the changes were made successfully.

Then, create a PR. The website czar will double check, then merge the PR if all looks well.

### 👋 Add a new person

1. Open the `config.yml` file
2. Navigate to the `authors` [key](https://github.com/carlosejimenez/lab-website/blob/main/config.yml#L12)
3. Under the `authors` key, copy and paste the below block, then replace the values in `<...>`
```
<username>:
  name: <name>
  pic: <link or path (see below for more details)>
  link: <URL to website>
  github: <Github Username>
  scholar: <Google Scholar URL>
  twitter: <Twitter Username>
```
4. Add your username to the `people` [list](https://github.com/carlosejimenez/lab-website/blob/main/content/people.md)
5. Launch the website, then check the "People" tab to confirm your profile was added

**Add a Profile Picture**

You may add either a link or a static asset as your `pic`.

- (Recommended) For a static asset...
  - Add your image to the `static/images/people` [folder](https://github.com/carlosejimenez/lab-website/tree/main/static/images/people)
  - Add the name of your image as the field of pic `i.e. pic: jy1682.jpg`
- For a link, paste the link (i.e. `pic: http://...`)

### ⌨️ Add a new post

1. Create a `.md` (markdown) file under the `content/posts/` directory.
2. Copy and paste the following text (include the top and bottom `---`'s) to the beginning of the file, then fill in the fields. This is your post metadata.
```
---
title:     # Post Title
date:      # YYYY-MM-DD format
draft:     # if `true`, post will be hidden
post_type: blog # Do not change
authors:   # list of ids from `config.yml`
---
```
3. Write the content for your blog post below the metadata in Markdown. If you're unfamiliar with Markdown, [this]() is a good place to start. You can also check out `example.md` in the `posts` folder and, after starting `hugo server`, preview it [here](http://localhost:1313/posts/example/).

### 📜 Add a new publication

1. Create a `.md` (markdown) file under the `content/publications/` directory.
2. In the markdown folder, copy and paste the following text (include the top and bottom `---`'s) to the beginning of the file, then fill in the fields. This is your publication metadata.
```
---
title:     # Paper title
date:      # YYYY-MM-DD format
draft:     # if `true`, post will be hidden
post_type: publication # Do not change
authors:   # list of ids from `config.yml`
venue:     # conference / journal / ArXiv

# Below are optional, but strongly recommended
code:      # Link to GitHub Repo
link:      # Link to paper
site:      # Link to project website

# Read more about `direct_link` below
direct_link: # URL
---
```

When the publication is clicked on the website, you can decide whether to
* Go to a post, where you can write a blog-style post about your paper OR
* Go to an external link of your choice

To do the former, do *not* include the `direct_link` field. You can then write markdown below the metadata as you would with a post.

To do the latter, include the `direct_link` field and assign the value to be a URL. If a reader clicks your publication on the website, they will be directed to the URL specified in `direct_link`.
