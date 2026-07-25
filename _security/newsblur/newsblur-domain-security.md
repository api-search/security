---
api_specs:
- filename: newsblur-authentication-api-openapi.yml
  format: yaml
  label: NewsBlur authentication API
  slug: newsblur-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newsblur/refs/heads/main/openapi/newsblur-authentication-api-openapi.yml
- filename: newsblur-classifiers-api-openapi.yml
  format: yaml
  label: NewsBlur classifiers API
  slug: newsblur-classifiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newsblur/refs/heads/main/openapi/newsblur-classifiers-api-openapi.yml
- filename: newsblur-feed-management-api-openapi.yml
  format: yaml
  label: NewsBlur feed-management API
  slug: newsblur-feed-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newsblur/refs/heads/main/openapi/newsblur-feed-management-api-openapi.yml
- filename: newsblur-feeds-api-openapi.yml
  format: yaml
  label: NewsBlur feeds API
  slug: newsblur-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newsblur/refs/heads/main/openapi/newsblur-feeds-api-openapi.yml
- filename: newsblur-import-export-api-openapi.yml
  format: yaml
  label: NewsBlur import-export API
  slug: newsblur-import-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newsblur/refs/heads/main/openapi/newsblur-import-export-api-openapi.yml
- filename: newsblur-social-api-openapi.yml
  format: yaml
  label: NewsBlur social API
  slug: newsblur-social-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newsblur/refs/heads/main/openapi/newsblur-social-api-openapi.yml
- filename: newsblur-stories-api-openapi.yml
  format: yaml
  label: NewsBlur stories API
  slug: newsblur-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newsblur/refs/heads/main/openapi/newsblur-stories-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: newsblur.com
  spf: true
hosts:
- cert_expires: Oct  3 03:05:00 2026 GMT
  host: www.newsblur.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Newsblur Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NewsBlur, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: NewsBlur
provider_slug: newsblur
slug: newsblur-domain-security
source_filename: newsblur-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.newsblur.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 03:05:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: newsblur.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newsblur/refs/heads/main/security/newsblur-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- RSS
- News
- Feed Reader
- Aggregator
- Social
- Content
- Media
- Open Source
- MCP
---
