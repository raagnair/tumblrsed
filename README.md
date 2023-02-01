# tumblrsed
An SPA that leverages Tumblr as a remote CMS

This allows you to spin up a website + blog quickly (~1 to 2mins) without worrying about purchasing and configuring Wordpress, or other local CMS solutions. The overall architecture is such that the client will open a simple index.html, which has JavaScript that queries the specified Tumblr blog, via the v1 API, and displays blog post previws (with pagination). When any preview is clicked, it will query the specific blog post's ID and display it in an "individual" page.

There is also custom behavior for a calendly-powered contact page.    

## Usage
Dowwnload index.html and search for "loremipsum" inside of it. Replace as necessary. 
For example loremipsum.tumblr.com needs to be replaced with whatever your blog name is. 

## Screenshot
![image](https://media.giphy.com/media/j8OPC4rhB2iVh3S8o3/giphy-downsized-large.gif)

## Caveats
**SEO**
Predictably, since this creates the illusion of a blog from a single html file and a remote Tumblr blog, SEO doesn't work great. There may be optimizations available through the use of Tumblr tags, or metadata, but I have not investigated it yet. 

**Blog post formatting**
Customizing text or images inside of a blog post is not ergonomic at all, given that it is returned as raw HTML from the API. You can _still_ write raw HTML in the Tumblr post, and it will show up in your website, but the Tumblr editor will add many useless custom HTML artifacts for their own display purposes. WARNING -- if you open up a post that has custom HTML through Tumblr's wysiwyg editor, you'll corrupt your formatting.
