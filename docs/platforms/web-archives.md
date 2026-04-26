---
icon: simple/internetarchive
---

# York University Libraries Wayback Machine

York University Libraries maintains a web archiving program to capture and preserve web content related to the university.

This includes:

- Content governed by the [York University Common Records Schedule](https://crs.apps06.yorku.ca/)
- Select crawls of York University web properties, when resources permit

Archived content is publicly accessible via [wayback.library.yorku.ca](https://wayback.library.yorku.ca/).

---

## Policy

- [Web Archiving Policy](https://www.library.yorku.ca/web/about-us/library-policies/web-archiving-policy/)  
  Defines the scope, and guidelines for web archiving activities.

---

## Software and Tools

YUL uses a combination of open-source tools and internal scripts to capture and serve web archives.

### Replay

- [pywb](https://github.com/webrecorder/pywb/)  
  Web archive replay system used to provide access to archived content.
- [YUL Wayback Configuration](https://codeberg.org/YorkUniversityLibraries/web-archives)  
  Local configuration and deployment of `pywb`.

---

### Capture

- [Browsertrix Crawler](https://github.com/webrecorder/browsertrix-crawler)  
  Headless browser-based crawler used for capturing modern web content.
- [YUL Crawl Scripts](https://codeberg.org/YorkUniversityLibraries/web-archiving-cron-scripts)  
  Scheduled jobs and automation scripts for running crawls using Browsertrix Crawler.
