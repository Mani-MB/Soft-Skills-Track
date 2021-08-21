# Caching
## What is Caching?

Caching is the process of storing copies of files in a cache, or temporary storage location so that they can be accessed more quickly. Technically, a cache is any temporary storage location for copies of files or data, but the term is often used in reference to Internet technologies. Web browsers cache HTML files, JavaScript, and images in order to load websites more quickly, while DNS servers cache DNS records for faster lookups, and CDN servers cache content to reduce latency.

## Why Caching is Important?

Caching is extremely important because it allows developers to achieve performance improvements, sometimes considerably. As mentioned earlier, this is vital.  
In particular, neither users nor developers want applications to take a long time to process requests. As developers, we would like to deploy the most performing version of our applications. And as users, we are willing to wait only for a few seconds, and sometimes even milliseconds. The truth is that no one loves wasting their time looking at loading messages.

## How Does Caching Work?


When we request a website or try to open apps, it will request data from the original service. Once we've loaded it, it will store pieces of the information in the caching server and the next time when we access it, it won't take much time because it directly gathers data from the caching server, not from the original server. A cache doesn’t store all the details. It just stores some, to help the page load faster. The other storage, the slower storage has all the data. Cache servers don’t offer a lot of space, it holds just enough to improve speed-wise.

[![Caching Process](https://paradoxmarketing.io/wp-content/uploads/2021/05/whatiscaching-img.jpeg)]()

## What are the benifits of caching?

- **Improved quality of experience**  
Caching can deliver material improvements in the quality of experience (QoE) provided by content providers to consumers.

- **Increased network and energy efficiency**  
Caching enables more efficient use of network capacity by reducing the number of ‘trips’ to request and serve content. This effect can significantly reduce the need for duplicated infrastructure deployment – resulting in significant cost savings and economic benefits for the entire Internet ecosystem. Furthermore, commercial caching providers can operate at scale, making extensive use of infrastructure shared between multiple customers, which is energy efficient. 

- **More dynamic competition and innovation**  
Access to caching services lowers barriers to entry for emerging content providers and supports these companies in delivering innovative services to consumers. Caching allows new or emerging content providers to provide a good user experience from service launch without making costly infrastructure investments, enabling them to compete with established players. 

## Different tyoes of Server Caching Strategies

**1. Cache-Aside**  

In this caching strategy, the cache is logically placed at the side and the application directly communicates with the cache and the database to know if the requested information is present or not. The cache is first checked by the application. If the information is found, it is marked as a cache hit, and so, it is read and returned to the client. If the information is not present, it is marked as a cache miss. The application queries the database for reading the data, returns the read data to the client, and then stores it in cache for future cache hits.

**2. Write-Through Cache**  

In this method, the information is first written to the cache before the main memory/database. The cache is logically in between the Application, through which the client interacts, and the database. Therefore, if a client requests anything the application does not have to check in the cache for its availability since it is already there. It directly retrieves from the cache memory and serves the client.

**3. Read-Through Cache**  

In this method, the cache sits inline with the database. Whenever there is a cache miss (meaning, the requested data isn’t in the cache), the missing data is populated from the database and gets returned to the application, so that the client is served.

**4. Write-Back**  

In this server caching strategy, the application writes the information to the cache that immediately acknowledges the changes, and after some delay, it writes back the data to the database. We can also call it write-behind.

**5. Write-Around**

In this case, the data is directly written in the database and only that data is stored into the cache which is read.

## More Caching Resources
1. [An Overview of Caching methods](https://www.cloudbees.com/blog/an-overview-of-caching-methods)

2. [HTTP caching](https://developer.mozilla.org/en-US/docs/Web/HTTP/Caching)
