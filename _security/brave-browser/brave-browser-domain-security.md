---
api_specs:
- filename: brave-browser-images-api-openapi.yml
  format: yaml
  label: Brave Images API
  slug: brave-browser-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave-browser/refs/heads/main/openapi/brave-browser-images-api-openapi.yml
- filename: brave-browser-local-api-openapi.yml
  format: yaml
  label: Brave Local API
  slug: brave-browser-local-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave-browser/refs/heads/main/openapi/brave-browser-local-api-openapi.yml
- filename: brave-browser-news-api-openapi.yml
  format: yaml
  label: Brave News API
  slug: brave-browser-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave-browser/refs/heads/main/openapi/brave-browser-news-api-openapi.yml
- filename: brave-browser-spellcheck-api-openapi.yml
  format: yaml
  label: Brave Spellcheck API
  slug: brave-browser-spellcheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave-browser/refs/heads/main/openapi/brave-browser-spellcheck-api-openapi.yml
- filename: brave-browser-suggest-api-openapi.yml
  format: yaml
  label: Brave Suggest API
  slug: brave-browser-suggest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave-browser/refs/heads/main/openapi/brave-browser-suggest-api-openapi.yml
- filename: brave-browser-summarizer-api-openapi.yml
  format: yaml
  label: Brave Summarizer API
  slug: brave-browser-summarizer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave-browser/refs/heads/main/openapi/brave-browser-summarizer-api-openapi.yml
- filename: brave-browser-videos-api-openapi.yml
  format: yaml
  label: Brave Videos API
  slug: brave-browser-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave-browser/refs/heads/main/openapi/brave-browser-videos-api-openapi.yml
- filename: brave-browser-web-api-openapi.yml
  format: yaml
  label: Brave Web API
  slug: brave-browser-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave-browser/refs/heads/main/openapi/brave-browser-web-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuemail ";"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:security@brave.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: brave.com
  spf: true
hosts:
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: brave.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: search.brave.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: api-dashboard.search.brave.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brave Browser Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brave, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Brave
provider_slug: brave-browser
slug: brave-browser-domain-security
source_filename: brave-browser-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: search.brave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: null\n- host: api-dashboard.search.brave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: brave.com\n  dnssec: true\n  caa:\n  - 0 issuemail \";\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@brave.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brave-browser/refs/heads/main/security/brave-browser-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Browser
- Search
- Privacy
- Chromium
- Web3
- AI
- Advertising
---
