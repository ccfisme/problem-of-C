# i++与++i在输出时不一样  

在学js的时候，我发现一个关于i++和++i的区分技巧：  

* i++的话是先输出i,然后i = i + 1；  
* ++i的话是先i = i + 1，然后输出i  

![屏幕快照 2021-12-27 下午2 29 56](https://user-images.githubusercontent.com/74129445/147445171-8ab109da-2bee-4540-b424-a3bbccc90ce4.png)  

后来我又看了自己的一些总结，发现并不是我想的那样，i++其实也是先i = i + 1，只不过i++ [返回的值是新建的一个临时的tmp值，保存的是i增加前的值](https://www.codenong.com/cs109606846/)  

![image](https://user-images.githubusercontent.com/74129445/147445370-8f53fa7c-5ecf-4da9-83bb-c964f4db8e0c.png)  

# i++不能作为左值  

![image](https://user-images.githubusercontent.com/74129445/147445766-1fd57ab1-e4ad-4254-91f4-0b6842806cea.png)



