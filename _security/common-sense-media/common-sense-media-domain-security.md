---
api_specs:
- filename: common-sense-media-reviews-api-openapi.yml
  format: yaml
  label: Common Sense Media Reviews API
  slug: common-sense-media-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/common-sense-media/refs/heads/main/openapi/common-sense-media-reviews-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: commonsensemedia.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: commonsense.org
  spf: true
hosts:
- cert_expires: Sep  3 15:30:58 2026 GMT
  host: www.commonsensemedia.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 13:49:30 2026 GMT
  host: api.commonsense.org
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Common Sense Media Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Common Sense Media, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Common Sense Media
provider_slug: common-sense-media
slug: common-sense-media-domain-security
source_filename: common-sense-media-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.commonsensemedia.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 15:30:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.commonsense.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 26 13:49:30 2026 GMT\n  hsts: null\ndomains:\n- domain: commonsensemedia.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: commonsense.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/common-sense-media/refs/heads/main/security/common-sense-media-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Apps
- Books
- Media
- Movies
- Non-Profit
- Podcasts
- Ratings
- Reviews
- Television
- Video Games
- YouTube
---
