---
api_specs:
- filename: restream-openapi.yml
  format: yaml
  label: Restream API
  slug: restream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restream/refs/heads/main/openapi/restream-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: restream.io
  spf: true
hosts:
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: restream.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: developers.restream.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 12:45:15 2026 GMT
  host: api.restream.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Restream Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Restream, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Restream
provider_slug: restream
slug: restream-domain-security
source_filename: restream-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: restream.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.restream.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.restream.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 12:45:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: restream.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/restream/refs/heads/main/security/restream-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Broadcast
- Chat
- Content Delivery
- Live Streaming
- Multistreaming
- Video Streaming
---
