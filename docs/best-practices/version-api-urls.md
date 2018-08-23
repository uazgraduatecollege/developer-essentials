# Best Practice: Version API URLs

## Description

Web-published APIs, including both dynamic web services as well as linked libraries (like jQuery plugins and CSS themes), should always use the release version as part of the URL.
Once published, the versioned URL will not be unpublished unless there is a compelling reason to do so (see Exceptions below).

## Rationale

Version control is a foundation of modern development teams. In the context of published web service APIs, it helps preserves backwards compatibility with client utilities that have not yet been updated.

## Implementation

Implementation may vary depending on how the resource is deployed.

### As Apache Aliases

Where each alias references a unique working copy of the project checked out against a specific release tag.

```
Alias /urlcheckr/0.1.0 /path/to/urlcheckr/0.1.0
Alias /urlcheckr/0.2.0 /path/to/urlcheckr/0.2.0
```

### As S3 Directory Paths

```
s3://a_bucket/gpacalculator/1.0.0/jquery.gpacalculator.js
s3://a_bucket/gpacalculator/1.1.0/jquery.gpacalculator.js
```

## Examples

The URLCheckr API is used by GradApp to check whether URLs in Program Descriptions are valid. There is currently one published release and one pending release, implemented using Apache aliases:

- https://api.grad.arizona.edu/urlcheckr/0.1.0/
- https://api.grad.arizona.edu/urlcheckr/0.2.0/

The jQuery GPA Calculator is the client-side Javascript library that renders the public-facing [GPA Calculator](https://grad.arizona.edu/tools/gpacalculator/), published as S3-backed CloudFront resources:

- https://cdn.grad.arizona.edu/gpacalculator/1.0.0/jquery.gpacalculator.js
- https://cdn.grad.arizona.edu/gpacalculator/1.1.0/jquery.gpacalculator.js

## Exceptions

On rare occasions, there may be good reason to unpublish an API or resource, for example, to mitigate a security vulnerability or an incompatibility introduced by a change to an underlying database schema. In such cases, we should try to preserve the URL and serve a brief explanation of why the resource is no longer available and where an updated version might be found.

## Other References

Versioning API URLs goes hand-in-hand with the practice of [versioning all code](best-practices/version-all-code.md).
