---
title: How to improve the search in Shodan
date: 2024-01-01 04:30:SS +/-TTTT
categories: []
tags: []     # TAG names should always be lowercase
---
Shodan is a well-known recon tool, but in larger scopes, it has so many results that it's hard to find something useful.

![Desktop View](/assets/img/shodan.png)

In this image searching for hostnames from Microsoft we got +100k results. It would be a TON of work going through 20 pages of results trying to find something.


<h3> That's when the 'facets' search comes into play</h3>

Facets are a set of filters, that can help with your search. Some of the basic filters are 'country', 'city', 'ssl cert', and so on.
![Desktop View](/assets/img/facets.png)

Personally, the filter that helps me the most to find some interesting stuff for pentests and bug bounties is the 'http.title'. In many cases there will be some repetitive title with an error message or a default response for pages without content. 

So instead of going through 20 pages of search, you will have a list that only shows 1 time each title, and it's filtered by occurrences.

By doing that we can go for the titles that only show up one or two times in the whole search, that's where we can find something misconfigured, a subdomain that shouldn't be public, internal dashboards, and many more. 

![Desktop View](/assets/img/facets2.png)

In this image, we can see that we have some titles that get our attention.

From now on you just gotta dig and look for more.
