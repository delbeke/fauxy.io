# fauxy.io
Fauxy.io Website

## Deploy

- Run `aws s3 sync . s3://fauxy-website  --acl public-read --delete --cache-control must-revalidate --exclude '.git/*' --exclude README.md`
- Update CloudFront `aws cloudfront create-invalidation --distribution-id ENJ23R37JM6XQ --paths "/*"`

``