---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: PeerTube REST API
  slug: peertube-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Chocobozzz/PeerTube/develop/support/doc/api/openapi.yaml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: joinpeertube.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: cpy.re
  spf: true
hosts:
- cert_expires: Sep 26 14:14:34 2026 GMT
  host: joinpeertube.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 22:00:37 2026 GMT
  host: docs.joinpeertube.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 10:43:39 2026 GMT
  host: peertube2.cpy.re
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Peertube Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PeerTube, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: PeerTube
provider_slug: peertube
slug: peertube-domain-security
source_filename: peertube-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: joinpeertube.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:14:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.joinpeertube.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 22:00:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: peertube2.cpy.re\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 10:43:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: joinpeertube.org\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: cpy.re\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peertube/refs/heads/main/security/peertube-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Video
- Decentralized
- Federation
- Open Source
- ActivityPub
- Self-Hosted
- Streaming
---
