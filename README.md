# F-Future Blog [![Build Status](https://travis-ci.com/f-future/f-future.svg?branch=master)](https://travis-ci.com/f-future/f-future) [![996.icu](https://img.shields.io/badge/link-996.icu-red.svg)](https://996.icu)

Github Page: https://f-future.github.io/f-future/

## Guidance

### How to add posts

#### With Nodejs installed

1. Run the following to setup:
   
   ```bash
   npm ci
   ```

2. Run the following command to add a new post:

   ```bash
   npx hexo new '<newtitle>'
   ```
 
   This will create a `<newtitle>.md` file under the `source/_posts` folder. 

3. Edit the Markdown file to complete the post.
4. Run the following command to preview changes at `http://localshot:4000`:

   ```bash
   npx hexo server
   ```

#### Without Nodejs installed

1. Manually create a `<title>.md` file under `source/_posts` folder.
2. Make sure to add a header section like below (only `title` is mandatory):

   ```markdown
   ---
   title: <title>
   date: 2020-08-01 16:54:00
   tags:
   ---
   ```

3. Edit the Markdown file to complete the post.

Either way, once you've done adding posts locally, commit and push it upstream (You may need to upload a feature branch and raise a [Pull Request](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request)). Once the change is merged into `master` branch, CI will run automatically, and all you need to do is wait for a second and refresh the blog page to see the changes.
