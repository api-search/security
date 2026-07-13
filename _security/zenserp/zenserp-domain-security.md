---
api_specs:
- filename: documentation
  format: yaml
  label: Zenserp Search API
  slug: search
  spec_type: OpenAPI
  url: https://app.zenserp.com/documentation
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zenserp.com
  spf: true
hosts:
- cert_expires: Aug 30 08:00:49 2026 GMT
  host: zenserp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 15 23:59:59 2027 GMT
  host: app.zenserp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zenserp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zenserp, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zenserp
provider_slug: zenserp
slug: zenserp-domain-security
source_filename: zenserp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zenserp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 08:00:49 2026 GMT\n  hsts: false\n- host: app.zenserp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 15 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: zenserp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenserp/refs/heads/main/security/zenserp-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- SERP
- Search Engine Results
- Google Search
- Web Scraping
- SEO
- Image Search
- News Search
- Shopping Search
- Maps
- YouTube Search
- Bing
- Yandex
- DuckDuckGo
- Geolocation
- Keyword Research
---
