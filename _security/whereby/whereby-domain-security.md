---
api_specs:
- filename: whereby-openapi.yml
  format: yaml
  label: Whereby REST API
  slug: whereby-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whereby/refs/heads/main/openapi/whereby-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@whereby.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: whereby.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@whereby.com"
  dmarc: false
  dnssec: false
  domain: whereby.dev
  spf: false
hosts:
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: whereby.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: api.whereby.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Whereby Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Whereby, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Whereby
provider_slug: whereby
slug: whereby-domain-security
source_filename: whereby-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: whereby.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.whereby.dev\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: whereby.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@whereby.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: whereby.dev\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@whereby.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whereby/refs/heads/main/security/whereby-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Video
- Communications
- Real-Time
- WebRTC
- Embedded
- Meetings
- Collaboration
---
