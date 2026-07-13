---
api_specs:
- filename: brave-search-api.yml
  format: yaml
  label: Brave Search API
  slug: brave-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave/refs/heads/main/openapi/brave-search-api.yml
- filename: brave-ads-api.yml
  format: yaml
  label: Brave Ads API
  slug: brave-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brave/refs/heads/main/openapi/brave-ads-api.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuemail ";"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:security@brave.com"
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
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: api.search.brave.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 21:21:48 2026 GMT
  host: ads-help.brave.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brave, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Brave
provider_slug: brave
slug: brave-domain-security
source_filename: brave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.search.brave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ads-help.brave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 21:21:48 2026 GMT\n  hsts: false\ndomains:\n- domain: brave.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuemail \";\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@brave.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brave/refs/heads/main/security/brave-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Search
- Advertising
- Privacy
- Browser
- AI
- LLM
---
