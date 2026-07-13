---
api_specs:
- filename: tivo-video-metadata-openapi.yml
  format: yaml
  label: TiVo Video Metadata API
  slug: tivo-video-metadata
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tivo/refs/heads/main/openapi/tivo-video-metadata-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tivo.com
  spf: true
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:devops@stoplight.io"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stoplight.io
  spf: true
hosts:
- cert_expires: Oct  2 17:40:42 2026 GMT
  host: business.tivo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: data.tivo.com
  https: false
- cert_expires: Oct  6 22:17:08 2026 GMT
  host: tivo.stoplight.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tivo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tivo, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tivo
provider_slug: tivo
slug: tivo-domain-security
source_filename: tivo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: business.tivo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 17:40:42 2026 GMT\n  hsts: false\n- host: data.tivo.com\n  https: false\n- host: tivo.stoplight.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:17:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tivo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: stoplight.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:devops@stoplight.io\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tivo/refs/heads/main/security/tivo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Entertainment
- Metadata
- Television
- Movies
- Music
- Streaming
---
