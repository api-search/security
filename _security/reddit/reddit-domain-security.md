---
api_specs:
- filename: reddit-ads-api-openapi.yml
  format: yaml
  label: Reddit Ads API
  slug: ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-ads-api-openapi.yml
- filename: reddit-account-api-openapi.yml
  format: yaml
  label: Reddit Account API
  slug: reddit-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-account-api-openapi.yml
- filename: reddit-accounts-api-openapi.yml
  format: yaml
  label: Reddit Accounts API
  slug: reddit-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-accounts-api-openapi.yml
- filename: reddit-ad-groups-api-openapi.yml
  format: yaml
  label: Reddit Ad Groups API
  slug: reddit-ad-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-ad-groups-api-openapi.yml
- filename: reddit-campaigns-api-openapi.yml
  format: yaml
  label: Reddit Campaigns API
  slug: reddit-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-campaigns-api-openapi.yml
- filename: reddit-conversions-api-openapi.yml
  format: yaml
  label: Reddit Conversions API
  slug: reddit-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-conversions-api-openapi.yml
- filename: reddit-custom-audiences-api-openapi.yml
  format: yaml
  label: Reddit Custom Audiences API
  slug: reddit-custom-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-custom-audiences-api-openapi.yml
- filename: reddit-flair-api-openapi.yml
  format: yaml
  label: Reddit Flair API
  slug: reddit-flair-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-flair-api-openapi.yml
- filename: reddit-funding-api-openapi.yml
  format: yaml
  label: Reddit Funding API
  slug: reddit-funding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-funding-api-openapi.yml
- filename: reddit-links-comments-api-openapi.yml
  format: yaml
  label: Reddit Links & Comments API
  slug: reddit-links-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-links-comments-api-openapi.yml
- filename: reddit-listings-api-openapi.yml
  format: yaml
  label: Reddit Listings API
  slug: reddit-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-listings-api-openapi.yml
- filename: reddit-messages-api-openapi.yml
  format: yaml
  label: Reddit Messages API
  slug: reddit-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-messages-api-openapi.yml
- filename: reddit-moderation-api-openapi.yml
  format: yaml
  label: Reddit Moderation API
  slug: reddit-moderation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-moderation-api-openapi.yml
- filename: reddit-oembed-api-openapi.yml
  format: yaml
  label: Reddit oEmbed API
  slug: reddit-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-oembed-api-openapi.yml
- filename: reddit-reporting-api-openapi.yml
  format: yaml
  label: Reddit Reporting API
  slug: reddit-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-reporting-api-openapi.yml
- filename: reddit-search-api-openapi.yml
  format: yaml
  label: Reddit Search API
  slug: reddit-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-search-api-openapi.yml
- filename: reddit-subreddits-api-openapi.yml
  format: yaml
  label: Reddit Subreddits API
  slug: reddit-subreddits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-subreddits-api-openapi.yml
- filename: reddit-targeting-api-openapi.yml
  format: yaml
  label: Reddit Targeting API
  slug: reddit-targeting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-targeting-api-openapi.yml
- filename: reddit-users-api-openapi.yml
  format: yaml
  label: Reddit Users API
  slug: reddit-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-users-api-openapi.yml
- filename: reddit-wiki-api-openapi.yml
  format: yaml
  label: Reddit Wiki API
  slug: reddit-wiki-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/openapi/reddit-wiki-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: reddit.com
  spf: true
hosts:
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: www.reddit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: oauth.reddit.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: ads-api.reddit.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reddit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reddit, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Reddit
provider_slug: reddit
slug: reddit-domain-security
source_filename: reddit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reddit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: oauth.reddit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: null\n- host: ads-api.reddit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: reddit.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reddit/refs/heads/main/security/reddit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- Communities
- Content
- Social-Media
- Social News
---
