# tumblrsed
An SPA that leverages Tumblr as a remote CMS

This allows you to spin up a website + blog quickly (~1 to 2mins) without worrying about purchasing and configuring Wordpress, or other local CMS solutions. The overall architecture is such that the client will open a simple index.html, which has JavaScript that queries the specified Tumblr blog, via the v1 API, and displays blog post previws (with pagination). When any preview is clicked, it will query the specific blog post's ID and display it in an "individual" page.
