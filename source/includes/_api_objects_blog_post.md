# <span class="jumptarget"> Store Content Reference </span>

Store Content APIs help merchants edit and publish blog posts and Web pages, improve SEO, and drive traffic to stores. They include Blog Posts, Blog Tags, Redirects, and Pages.

## <span class="jumptarget"> Blog Posts </span>

A content entry in the store’s blog.

### <span class="jumptarget"> Blog Post Object – Properties </span>

| Name | Type | Description |
| --- | --- | --- |
| id | int |  |
| title | string |  |
| url | string |  |
| preview_url | string |  |
| body | string |  |
| tags | array of strings |  |
| summary | string |  |
| is_published | boolean |  |
| published_date | date string, or object | When including the blog post's `published_date` in `PUT` or `POST` requests, supply it as a flat date string in valid <a href="http://tools.ietf.org/html/rfc2822#section-3.3" target="_blank">RFC 2822</a> or <a href="https://en.wikipedia.org/wiki/ISO_8601" target="_blank">ISO 8601</a> format. <br> <br> In GET requests, the `published_date` is returned as an object, whose members are: `date` (date string); `timezone_type` (integer); and `timezone` (string representing an hours:minutes offset, in the format `"+hh:mm"` or `"-hh:mm"`). |
| published_date_iso8601 | date string | Published date in <a href="https://en.wikipedia.org/wiki/ISO_8601" target="_blank">ISO 8601</a> format. |
| meta_description | string |  |
| meta_keywords | string |  |
| author | string |  |
| thumbnail_path | string |  |
