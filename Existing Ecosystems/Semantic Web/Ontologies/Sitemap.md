Sitemap.rdf is an update to the Sitemap.xml file.

```

@prefix sitemap: <http://www.sitemaps.org/schemas/sitemap/0.9/> .
@prefix xhtml: <http://www.w3.org/1999/xhtml/> .

<http://example.com/sitemap.rdf> a sitemap:Sitemap ;
  sitemap:url [
    a sitemap:Url ;
    sitemap:loc <http://example.com/> ;
    sitemap:lastmod "2022-12-28T12:00:00+00:00"^^xsd:dateTime ;
    sitemap:changefreq sitemap:weekly ;
    sitemap:priority 1.0
  ] .

<http://example.com/sitemap.rdf> a sitemap:Sitemap ;
  sitemap:url [
    a sitemap:Url ;
    sitemap:loc <http://example.com/about> ;
    sitemap:lastmod "2022-12-28T12:00:00+00:00"^^xsd:dateTime ;
    sitemap:changefreq sitemap:weekly ;
    sitemap:priority 0.8
  ] .

@prefix sitemap: <http://www.sitemaps.org/schemas/sitemap/0.9/> .
@prefix xhtml: <http://www.w3.org/1999/xhtml/> .

<http://example.com/sitemap.rdf> a sitemap:Sitemap ;
  sitemap:url [
    a sitemap:Url ;
    sitemap:loc <http://example.com/> ;
    sitemap:lastmod "2022-12-28T12:00:00+00:00"^^xsd:dateTime ;
    sitemap:changefreq sitemap:weekly ;
    sitemap:priority 1.0 ;
    sitemap:allow true
  ] .

<http://example.com/sitemap.rdf> a sitemap:Sitemap ;
  sitemap:url [
    a sitemap:Url ;
    sitemap:loc <http://example.com/> ;
    sitemap:lastmod "2022-12-28T12:00:00+00:00"^^xsd:dateTime ;
    sitemap:changefreq sitemap:weekly ;
    sitemap:priority 1.0 ;
    sitemap:allow true
  ] .

<http://example.com/sitemap.rdf> a sitemap:Sitemap ;
  sitemap:url [
    a sitemap:Url ;
    sitemap:loc <http://example.com/about> ;
    sitemap:lastmod "2022-12-28T12:00:00+00:00"^^xsd:dateTime ;
    sitemap:changefreq sitemap:weekly ;
    sitemap:priority 0.8 ;
    sitemap:allow true
  ] .

<http://example.com/sitemap.rdf> a sitemap:Sitemap ;
  sitemap:url [
    a sitemap:Url ;
    sitemap:loc <http://example.com/private> ;
    sitemap:lastmod "2022-12-28T12:00:00+00:00"^^xsd:dateTime ;
    sitemap:changefreq sitemap:weekly ;
    sitemap:priority 0.5 ;
    sitemap:allow false
  ] .



```

Robots.txt

```

@prefix robots: <http://www.robotstxt.org/ontology/robots#> .

<http://example.com/robots.rdf> a robots:RobotsFile ;
  robots:rule [
    a robots:Rule ;
    robots:userAgent "Googlebot" ;
    robots:disallow "/private"
  ] .

<http://example.com/robots.rdf> a robots:RobotsFile ;
  robots:rule [
    a robots:Rule ;
    robots:userAgent "*" ;
    robots:allow "/public"
  ] .

```

This example defines a `robots.txt` file for a website with two rules. The first rule specifies that the Googlebot should not crawl the `/private` directory. The second rule specifies that all other user agents are allowed to crawl the `/public` directory.

You can add additional rules as needed by adding more `robots:rule` statements to the `robots:RobotsFile`. For example, you could add a rule that disallows all user agents from crawling a `/sensitive` directory, like this:

```

@prefix robots: <http://www.robotstxt.org/ontology/robots#> .

<http://example.com/robots.rdf> a robots:RobotsFile ;
  robots:rule [
    a robots:Rule ;
    robots:userAgent "Googlebot" ;
    robots:disallow "/private"
  ] .

<http://example.com/robots.rdf> a robots:RobotsFile ;
  robots:rule [
    a robots:Rule ;
    robots:userAgent "*" ;
    robots:allow "/public"
  ] .

<http://example.com/robots.rdf> a robots:RobotsFile ;
  robots:rule [
    a robots:Rule ;
    robots:userAgent "*" ;
    robots:disallow "/sensitive"
  ] .

```

SiteIndex

```
@prefix siteindex: <http://www.siteindex.org/ontology/siteindex#> .
@prefix xhtml: <http://www.w3.org/1999/xhtml/> .

<http://example.com/siteindex.rdf> a siteindex:SiteIndex ;
  siteindex:url [
    a siteindex:Url ;
    siteindex:loc <http://example.com/> ;
    siteindex:lastmod "2022-12-28T12:00:00+00:00"^^xsd:dateTime
  ] .

<http://example.com/siteindex.rdf> a siteindex:SiteIndex ;
  siteindex:url [
    a siteindex:Url ;
    siteindex:loc <http://example.com/about> ;
    siteindex:lastmod "2022-12-28T12:00:00+00:00"^^xsd:dateTime
  ] .


```
You can add additional URLs to the `siteindex` by adding more `siteindex:url` statements to the `siteindex:SiteIndex`. For example, you could add a page for contact information like this:

```
@prefix siteindex: <http://www.siteindex.org/ontology/siteindex#> .
@prefix xhtml: <http://www.w3.org/1999/xhtml/> .

<http://example.com/siteindex.rdf> a siteindex:SiteIndex ;
  siteindex:url [
    a siteindex:Url ;
    siteindex:loc <http://example.com/> ;
    siteindex:lastmod "2022-12-28T12:00:00+00:00"^^xsd:dateTime
  ] .

<http://example.com/siteindex.rdf> a siteindex:SiteIndex ;
  siteindex:url [
    a siteindex:Url ;
    siteindex:loc <http://example.com/about> ;
    siteindex:lastmod "2022-12-28T12:00:00+00:00"^^xsd:dateTime
  ] .

<http://example.com/siteindex.rdf> a siteindex:SiteIndex ;
  siteindex:url [
    a siteindex:Url ;
    siteindex:loc <http://example.com/contact> ;
    siteindex:lastmod "2022-12-28T12:00:00+00:00"^^xsd:dateTime
  ] .
```

