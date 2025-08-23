# CDN 

## Overview 

CDN is a content delivery network, which means that it is a system where the servers are present globally. These servers store the website content, which helps users to retrieve the information faster. Unlike single-origin servers, the servers in CDN are POPs. POPs (Points of presence) are the intentionally located caching servers. It brings website content closer to the user, helping increase latency and improving website loading speed. 

Example: Google Cloud CDN, Amazon CloudFront 

 

## How a CDN works: 

Metaphorically speaking, CDN is like a delivery hub. Instead of users getting content from the main warehouse (origin server), they get it from a local shop (nearest CDN edge server). 
- Origin server: This is where your original data/ files are located. 
- Edge server (CDN nodes): servers located around the world. Store cached copies of the website’s files. 
- What happens when a user visits a site with a CDN? A user enters a domain, and the user is in a different location other than on the original server.
- CDN uses Geo-D   Geo-DNS. It is a system which helps locate the user and helps send the user’s request to the nearest CDN edge server. There is the advantage of requests being sent to different IP addresses rather than to the same server.  
- Cache check: The edge server checks if the server already has the content which is requested by the user. If yes, it immediately sends it to the user; otherwise it fetches it from the original server and stores a copy of it in the cache, then delivers it to the user. 

## Key Features: 
- Content caching
- Load balancing
- DDoS (Distributed denial of service) protection and security.
 
## Benefits and Use Cases: 
- Faster website loading (important for e-commerce)
- CDNs are very important in SaaS product delivery.
- SaaS apps rely on real-time access (dashboards, APIs, forms). 
- CDN caches static assets (CSS, JS, images, libraries) at edge servers, so they load instantly. 
- For dynamic data (API calls, DB queries), CDN routes requests to the nearest server for lower l-atency. 

## What can be cached? 

- Static content: 
We can cache Images, CSS, JavaScript, fonts, videos, PDFs, HTML pages. 
- Dynamic content: 
Can be cached with short expiry or edge-side logic.  

## Techniques CDNs use to reduce latency: 
- Geo-proximity – Content served from the closest edge server.
- Caching – Saves frequently used files at edges.
- Load balancing – Distributes requests across multiple servers to avoid overload.
- Compression – Gzip/Brotli compression for smaller transfer size.
- Protocol optimization – Uses HTTP/2, HTTP/3 (QUIC) for faster connections.
- Image & Video Optimization – Auto-resizing, WebP conversion, adaptive streaming.

  ## References
  - https://www.youtube.com/watch?v=zw7VwIlkPPc
  - https://www.youtube.com/watch?v=b2scqJYSFf0
  - www.google.com
  - [htttps.chatgpt.com](https://chat.openai.com/auth/login)
