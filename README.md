- To create a new post run `hexo new <post name>` the name will be the title and the url path but you can change the title that appears on the actual post in the yaml config on top of the post

- Work off of the `develop` branch but don't merge into master, when you want to publish the post run `hexo generate -d` from the develop branch, this will take the latest from develop, and push it to github, on master it will have the generated files instead.

- Use imagemagick to compress imagery. Such as `magick IMG.jpg -scale 800x800 IMG.jpg` For the thumbnail images, save them in `source/assets`

- For images that are to be used inside the post, save them in `source/_posts/<post name>` in order to compress them you can run something like: `for X in *.jpeg; do magick "$X" -scale 400x400 "$X"; done`

- User `hexo server` to run