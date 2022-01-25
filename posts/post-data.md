```xml
<b:loop values='data:posts' var='post'>
  <!--  post thumbnail -->
  <img expr:src='data:post.featuredImage'/> 
  or
  <img expr:src='data:post.thumbnailUrl'/> 
  
  <!--  post url -->
  <a expr:src='data:post.url'> <data:post.url/> </a> 
  
  <!-- post content -->
  <h1><data:post.title/></h1>
  <p><data:post.body/></p> 
</b:loop>
```
