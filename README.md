# tumblrsed
An SPA that leverages Tumblr as a remote CMS

This allows you to spin up a website + blog quickly (~1 to 2mins) without worrying about purchasing and configuring Wordpress, or other local CMS solutions. The overall architecture is such that the client will open a simple index.html, which has JavaScript that queries the specified Tumblr blog, via the v1 API, and displays blog post previws (with pagination). When any preview is clicked, it will query the specific blog post's ID and display it in an "individual" page.

There is also custom behavior for a calendly-powered contact page.    

## Usage
Dowwnload index.html and search for "loremipsum" inside of it. Replace as necessary. 
For example loremipsum.tumblr.com needs to be replaced with whatever your blog name is. 

## Screenshots
![image](https://user-images.githubusercontent.com/7918609/215941698-2ba0d9f5-3605-4a34-9e54-d62d192eb2e6.png)
![image](https://user-images.githubusercontent.com/7918609/215941724-677503bc-82f2-40f7-a132-b03311262718.png)

## Caveats
Predictably, since this creates the illusion of a blog from a single html file and a remote Tumblr blog, SEO doesn't work great. There may be optimizations available through the use of Tumblr tags, or metadata, but I have not investigated it yet. 
