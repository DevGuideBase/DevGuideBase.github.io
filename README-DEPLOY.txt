DevToolkit Hub - static site (22,106 articles, 165 hubs, 11 categories)
=======================================================================

WHAT IS INSIDE
  /                          home: latest published posts, two ads (468x60 on top, 300x250 after the 9th card)
  /{tool}/{post}.html        22,106 article pages (two ads each, related posts from the same hub)
  /{tool}/{hub}/             165 hub pages, every post of the hub on one page, no pagination, two ads
  /category/{tool}/          11 category pages, every post on one page, no pagination, two ads
  /hubs/                     index of all hubs
  /page/*.html               DMCA, Contact, Privacy Policy, Copyright
  /sitemap.xml               index -> sitemap-pages.xml, sitemap-categories.xml, sitemap-hub-001..165-*.xml
  /schedule.csv, *.xlsx      publish manifest (NOT published: the workflow leaves it out)

HOW IT WAS TRIMMED
  33,000 posts -> 22,106. The 10,894 posts with the least original text (most sentences shared with other posts)
  were taken out, thinnest first, keeping at least 100 posts in every hub, until the site fit under 890 MB.
  Folder size: about 886 MB.

DEPLOY (GitHub Pages)
  1. Repository named <account>.github.io, Public.
  2. Copy ALL contents of this folder to the repository root (keep .nojekyll, .github/, the Google verification file).
  3. Settings -> Pages -> Source: GitHub Actions. The workflow .github/workflows/deploy-pages.yml publishes only the
     site files (it leaves out schedule.csv, *.xlsx, README-DEPLOY.txt, _build-manifest.json).
  4. Search Console: submit sitemap.xml.

SCHEDULE
  schedule.csv / xlsx list the remaining 22,106 posts (993 Published, 21,113 Scheduled). If you deploy everything at
  once (recommended) the schedule is only a record.
