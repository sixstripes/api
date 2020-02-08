---
layout: default
title: Home
nav_order: 1
description: "Just the Docs is a responsive Jekyll theme with built-in search that is easily customizable and hosted on GitHub Pages."
permalink: /
---

# Starting out with the API
{: .fs-9 }

Making way for representation through data, the Sixstripes API enables reseachers, jornalists, students, businesses and you to explore, understand and connect to a more diverse world.
{: .fs-6 .fw-300 }

---

## Signing up

Web API also provides access to user related data, like playlists and music that the user saves in the Your Music library. Such access is enabled through selective authorization, by the user.

```
The base address of Web API is https://api.spotify.com.
The API provides a set of endpoints, each with its own unique path.
```

## Authentication

Rate Limiting enables Web API to share access bandwidth to its resources equally across all users

1. Rate limiting is applied as per application based on Client ID, and regardless of the number of users who use the application simultaneously.

2. To reduce the amount of requests, use endpoints that fetch multiple entities in one request. For example: If you often request single tracks, albums, or artists, use endpoints such as Get Several Tracks, Get Several Albums or Get Several Artists, instead

If Web API returns status code 429, it means that you have sent too many requests. When this happens, check the Retry-After header, where you will see a number displayed. This is the number of seconds that you need to wait, before you try your request again.