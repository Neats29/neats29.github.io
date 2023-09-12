- To create a new post run `hexo new <post name>` the name will be the title and the url path but you can change the title that appears on the actual post in the yaml config on top of the post

- Work off of the `develop` branch, push to develop but don't merge into master, when you want to publish the post, commit and run `hexo generate -d` from the develop branch, this will take the latest from develop, and push it to github, on master it will have the generated files instead.

- Use imagemagick to compress imagery. Such as `magick IMG.jpg -scale 400x400 IMG.jpg` For the thumbnail images, save them in `source/assets`
- use `ls -s` to check the size of the images

- For images that are to be used inside the post, save them in `source/_posts/<post name>` in order to compress them you can run something like: `for X in *.jpeg; do magick "$X" -scale 400x400 "$X"; done`

* Use `hexo server` to run
* if `hexo` is not installed globally you can run `npx hexo server` instead

- use [this tool](https://opengraphr.com/open-graph-debugger) to preview the thumbnail image 

---

- To create a new page run `hexo new page <name>`

- `cmd shift v` to preview a markdown file

- if you need to change a css attribute, make the change in `themes/phantom-non-jekyll/source/sass/*`

- The theme https://github.com/klugjo/hexo-theme-phantom

**2022 update:**
The hexo-renderer-sass package which is a dependency for the theme, uses node-sass which has been deprecated. There is a fix for it but it hasn't been merged, so I used [this fork](https://github.com/knksmith57/hexo-renderer-sass/pull/46) for the time being.


<!-- 
sudo chown -R $(whoami) .
chmod -R u+rwx . 
 -->