# Caching
Caching helps increase speed by providing a small data store with faster access

Helpful when you have more **Reads** than **Writes**

## Caching Architecture
1. Have a in-memory cache on app/web servers. Must scale w/ web servers
2. Have dedicated caching servers. Can scale independently. 

Things to consider
- Expiration policy
- Hotspots. If a few items are being more targeted than others in a cache
- Cold-Start. How to start the cache? or the caching layer gets deleted. Needs time to be primed.
## Eviction policies
LRU - Least Recently Used
LFU - Least Frequently Used
FIFO - First In First Out

## Caching Tech
MemCache - InMemory k/V store, open source
Redis - more complex and advanced than memcache

Amazon ElastiCache - Fully managed Redis/MemCached

## Content Delivery Networks (CDN)
- Geographically destributed (edge locations)
- Useful for static content (static web pages). Not for general caching
- Very expensive
- Increases Speed for content access
- Decreases Load on servers (as they are handled by CDN)
- Security through obscurity (less direct access with Server)
- Be careful on what it is used for


