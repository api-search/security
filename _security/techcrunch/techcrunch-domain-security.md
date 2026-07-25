---
api_specs:
- filename: techcrunch-authors-api-openapi.yml
  format: yaml
  label: TechCrunch Authors API
  slug: techcrunch-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/techcrunch/refs/heads/main/openapi/techcrunch-authors-api-openapi.yml
- filename: techcrunch-categories-api-openapi.yml
  format: yaml
  label: TechCrunch Categories API
  slug: techcrunch-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/techcrunch/refs/heads/main/openapi/techcrunch-categories-api-openapi.yml
- filename: techcrunch-comments-api-openapi.yml
  format: yaml
  label: TechCrunch Comments API
  slug: techcrunch-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/techcrunch/refs/heads/main/openapi/techcrunch-comments-api-openapi.yml
- filename: techcrunch-media-api-openapi.yml
  format: yaml
  label: TechCrunch Media API
  slug: techcrunch-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/techcrunch/refs/heads/main/openapi/techcrunch-media-api-openapi.yml
- filename: techcrunch-pages-api-openapi.yml
  format: yaml
  label: TechCrunch Pages API
  slug: techcrunch-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/techcrunch/refs/heads/main/openapi/techcrunch-pages-api-openapi.yml
- filename: techcrunch-posts-api-openapi.yml
  format: yaml
  label: TechCrunch Posts API
  slug: techcrunch-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/techcrunch/refs/heads/main/openapi/techcrunch-posts-api-openapi.yml
- filename: techcrunch-search-api-openapi.yml
  format: yaml
  label: TechCrunch Search API
  slug: techcrunch-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/techcrunch/refs/heads/main/openapi/techcrunch-search-api-openapi.yml
- filename: techcrunch-tags-api-openapi.yml
  format: yaml
  label: TechCrunch Tags API
  slug: techcrunch-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/techcrunch/refs/heads/main/openapi/techcrunch-tags-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: techcrunch.com
  spf: true
- caa:
  - 0 iodef "mailto:caa@wordpress.org"
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wordpress.org
  spf: true
hosts:
- cert_expires: Aug 20 04:24:49 2026 GMT
  host: techcrunch.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 19:43:58 2026 GMT
  host: developer.wordpress.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Techcrunch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TechCrunch, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TechCrunch
provider_slug: techcrunch
slug: techcrunch-domain-security
source_filename: techcrunch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: techcrunch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 04:24:49 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: developer.wordpress.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 19:43:58 2026 GMT\n  hsts: false\ndomains:\n- domain: techcrunch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: wordpress.org\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:caa@wordpress.org\"\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/techcrunch/refs/heads/main/security/techcrunch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Media
- News
- Startups
- Technology News
- Venture Capital
---
