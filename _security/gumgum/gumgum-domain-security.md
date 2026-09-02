---
api_specs:
- filename: gumgum-image-api-openapi.yml
  format: yaml
  label: GumGum Image API
  slug: gumgum-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumgum/refs/heads/main/openapi/gumgum-image-api-openapi.yml
- filename: gumgum-intravideo-api-openapi.yml
  format: yaml
  label: GumGum Intravideo API
  slug: gumgum-intravideo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumgum/refs/heads/main/openapi/gumgum-intravideo-api-openapi.yml
- filename: gumgum-page-api-openapi.yml
  format: yaml
  label: GumGum Page API
  slug: gumgum-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumgum/refs/heads/main/openapi/gumgum-page-api-openapi.yml
- filename: gumgum-text-api-openapi.yml
  format: yaml
  label: GumGum Text API
  slug: gumgum-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumgum/refs/heads/main/openapi/gumgum-text-api-openapi.yml
- filename: gumgum-video-api-openapi.yml
  format: yaml
  label: GumGum Video API
  slug: gumgum-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gumgum/refs/heads/main/openapi/gumgum-video-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gumgum.com
  spf: true
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jira.com
  spf: true
hosts:
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: gumgum.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: gumgum.jira.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: verity-api.gumgum.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gumgum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GumGum, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GumGum
provider_slug: gumgum
slug: gumgum-domain-security
source_filename: gumgum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gumgum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gumgum.jira.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: verity-api.gumgum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: gumgum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: jira.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gumgum/refs/heads/main/security/gumgum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- AdTech
- Contextual Advertising
- Brand Safety
- content-classification
- Computer-Vision
- Natural Language Processing
- Video Analysis
- Image Analysis
- Connected TV
- Header Bidding
- Programmatic Advertising
- iab-taxonomy
- Content Moderation
---
