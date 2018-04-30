## Structure A
Classic structure with assets in the static folder.

#### Pros
Clear separation of content files that are processed and assets that are static.
Flat content tree.

#### Cons

Managing assets in the static folder can be a pain: If we put all images in
one folder it is difficult to tell which images are still in use and which images
could be deleted. We could replicate the entire structure of the content for
images but this is also a lot of work to maintain.
References to images are long and may lead to mistakes
(for example /images/blog/firstpost/post-image-1.jpg).



## Structure B
Keep content and assets together.
#### Pros

Content files and corresponding assets are in one folder. This is very clean
from a content perspective since I consider images of a blog post also as
content (not processd, but still content). For example, we can create a zip
file from a blog post folder with markdown and images and we have everything
that belongs to that blog post.
Images in the content folder are also much easier to maintain.
For example, if we delete a blog post, we can savely delete the blog posts
images as they live in the same folder.
References to images are short (for example post-image-1.jpg). This also
means that Github finds and displays the images when the markdown file is opened.

#### Cons

Content contains a mix of files to be processed (markdown) and static files
(images). If we did some image optimization/resizing/cropping, we could argue
that images are processed as well and thus belong to the content folder.
A lot of folders to manage in the content directory

### For details check the link
    https://discourse.gohugo.io/t/discussion-content-organization-best-practice/6360


Thanks to
## Marco Jakob
@marcojakob
