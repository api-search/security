---
api_specs:
- filename: frameio-v4-openapi.json
  format: json
  label: Frame.io V4 API
  slug: frameio-v4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frameio/refs/heads/main/openapi/frameio-v4-openapi.json
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: frame.io
  spf: true
hosts:
- cert_expires: Sep 26 23:45:57 2026 GMT
  host: www.frame.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: api.frame.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Frameio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Frame.io, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Frame.io
provider_slug: frameio
slug: frameio-domain-security
source_filename: frameio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.frame.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:45:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.frame.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: frame.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frameio/refs/heads/main/security/frameio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Media
- Video
- Collaboration
- Review and Approval
- Media Production
- Adobe
- Content
---
