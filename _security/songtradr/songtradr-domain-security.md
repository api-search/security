---
api_specs:
- filename: songtradr-allowed-values-api-openapi.yml
  format: yaml
  label: Songtradr Allowed Values API
  slug: songtradr-allowed-values-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/songtradr/refs/heads/main/openapi/songtradr-allowed-values-api-openapi.yml
- filename: songtradr-similarity-vector-controller-api-openapi.yml
  format: yaml
  label: Songtradr Similarity Vector Controller API
  slug: songtradr-similarity-vector-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/songtradr/refs/heads/main/openapi/songtradr-similarity-vector-controller-api-openapi.yml
- filename: songtradr-user-api-openapi.yml
  format: yaml
  label: Songtradr User API
  slug: songtradr-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/songtradr/refs/heads/main/openapi/songtradr-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: songtradr.com
  spf: true
hosts:
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: www.songtradr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 17:11:36 2026 GMT
  host: api.songtradr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Songtradr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Songtradr, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Songtradr
provider_slug: songtradr
slug: songtradr-domain-security
source_filename: songtradr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.songtradr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: false\n- host: api.songtradr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 17:11:36 2026 GMT\n  hsts: null\ndomains:\n- domain: songtradr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/songtradr/refs/heads/main/security/songtradr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Music
- Music Licensing
- Sync Licensing
- Music Metadata
- audio-tagging
- Semantic Search
- Machine-Learning
- Media
- Entertainment
- Rights Management
- Audio
---
