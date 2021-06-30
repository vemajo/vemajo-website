# Usage

Install Hugo (https://gohugo.io/)

```
sudo apt install hugo
```

Clone the repo to yuor local machine:

```
git clone https://github.com/vemajo/vemajo-website.git
cd vemajo-website
git checkout -b "feat/new-awesome-post"
```

Create or modify content.:

```
hugo new content/posts/post-4.md
vi content/posts/post-4.md
```

Hugo supports markdown language:

```
title: "Example title"
date: 2021-06-18T13:59:28+03:00
draft: false
---

# Example heading

Example paragraph. Lirumloremipsum asdf

## Example heading 2
```

After that you can test out the changes by running a local server:

```
hugo server -D
```

If you are happy with the changes, compile the webpage and push it to remote branch:

```
hugo -D
git add --a
git commit
git push origin
```

Create a pull request. CD pipeline will deploy it automatically to Cloud Storage after the merge.
