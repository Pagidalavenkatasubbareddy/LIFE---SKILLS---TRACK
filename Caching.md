# Caching

## What is caching ?

   * The same things happen in the system. In a system accessing data from primary memory (RAM) is faster than accessing data from secondary memory (disk). 
   *  Caching acts as the local store for the data and retrieving the data from this local or temporary storage is easier and faster than retrieving it from the database.
   * Consider it as a short-term memory that has limited space but is faster and contains the most recently accessed items.
   * So If you need to rely on a certain piece of data often then cache the data and retrieve it faster from the memory rather than the disk.

##  How Does Cache Work ?

   * web application stores data in a database. When a client requests some data, it is fetched from the database and then it is returned to the user. 
   * Reading data from the database needs network calls and I/O operation which is a time-consuming process. 
   * Cache reduces the network call to the database and speeds up the performance of the system. 

## Where Cache Can be Added ?

   * Caching is used in almost every layer of computing.
   * In hardware, for example, you have various layers of cache memory.
   * You have layer 1 cache memory which is the CPU cache memory, then you have layer 2 cache memory and finally, you would have the regular RAM (random access memory).
   * You also have to cache in the operating systems such as caching various kernel extensions or application files.
   * You also have caching in a web browser to decrease the load time of the website. 


### Here is how using cache helps to resolve this problem 

   * To reduce the number of calls to the database, we can use cache and the tweets can be provided much faster.
   * In a typical web application, we can add an application server cache, and an in-memory store like Redis alongside our application server.
   * When the first time a request is made a call will have to be made to the database to process the query. This is known as a cache miss.
   * Before giving back the result to the user, the result will be saved in the cache.
   * When the second time a user makes the same request, the application will check your cache first to see if the result for that request is cached or not.
   * If it is then the result will be returned from the in-memory store. This is known as a cache hit.
   * The response time for the second time request will be a lot less than the first time. 
  
##  Key points to understand Caching
Caching can be used in a variety of different systems, including web applications, databases, and operating systems. In each case, caching works by storing data that is frequently accessed in a location that is closer to the user or application. This can include storing data in memory or on a local hard drive.

###  => How it works:
   * When data is requested, the system first checks if the data is stored in the cache.
   * If it is, the system retrieves the data from the cache rather than from the original source.
   * This can significantly reduce the time it takes to access the data.
###  => Types of caching:
   * There are several types of caching, including in-memory caching, disk caching, and distributed caching.
   * In-memory caching stores data in memory, while disk caching stores data on a local hard drive.
   * Distributed caching involves storing data across multiple systems to improve availability and performance.
###  => Cache eviction:
   * Caches can become full over time, which can cause performance issues.
   * To prevent this, caches are typically designed to automatically evict older or less frequently accessed data to make room for new data.
###  => Cache consistency:
   * Caching can introduce issues with data consistency, particularly in systems where multiple users or applications are accessing the same data.
   * To prevent this, systems may use cache invalidation techniques or implement a cache consistency protocol to ensure that data remains consistent across all users and applications.

## What are the Advantages of using Caching ?

*  Caching optimizes resource usage, reduces server loads, and enhances overall scalability, making it a valuable tool in software development.
  
=>  Improved performance:   Caching can significantly reduce the time it takes to access frequently accessed data, which can improve system performance and responsiveness.

=> Reduced load on the original source:   By reducing the amount of data that needs to be accessed from the original source, caching can reduce the load on the source and improve its scalability and reliability.

=> Cost savings:  Caching can reduce the need for expensive hardware or infrastructure upgrades by improving the efficiency of existing resources.

##  What are the Disadvantages of using Caching ?

* Despite its advantages, caching comes with drawbacks also and some of them are:

=> Data inconsistency: If cache consistency is not maintained properly, caching can introduce issues with data consistency.

=> Cache eviction issues: If cache eviction policies are not designed properly, caching can result in performance issues or data loss.

=> Additional complexity: Caching can add additional complexity to a system, which can make it more difficult to design, implement, and maintain.

## Conclusion

*   Caching is becoming more common nowadays because it helps make things faster and saves resources.
*   The internet is witnessing an exponential growth in content, including web pages, images, videos, and more.
*   Caching helps reduce the load on servers by storing frequently accessed content closer to the users, leading to faster load times.
*   Real-time applications, such as online gaming, video streaming, and collaborative tools, demand low-latency interactions.
*   Caching helps in delivering content quickly by storing and serving frequently accessed data without the need to fetch it from the original source every time.


## References 
=> [Caching learn in MDN docs](https://developer.mozilla.org/en-US/docs/Web/API/Cache)

=> [Geeks for Geeks to understanding Caching ](https://www.geeksforgeeks.org/caching-system-design-concept-for-beginners/)

=> [ searching in Cloudflare to understanding Caching ](https://www.cloudflare.com/learning/cdn/what-is-caching/)

=> [understanding Caching in fortinet ](https://www.fortinet.com/resources/cyberglossary/what-is-caching)