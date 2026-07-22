---
api_specs:
- filename: xbow-openapi-original.json
  format: json
  label: XBOW API
  slug: xbow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xbow/refs/heads/main/openapi/xbow-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: xbow.com
  spf: true
hosts:
- cert_expires: Sep 22 15:22:40 2026 GMT
  host: xbow.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 17:21:21 2026 GMT
  host: docs.xbow.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 14:15:26 2026 GMT
  host: console.xbow.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xbow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xbow, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Xbow
provider_slug: xbow
slug: xbow-domain-security
source_filename: xbow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xbow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 15:22:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.xbow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 17:21:21 2026 GMT\n  hsts: false\n- host: console.xbow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 14:15:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: xbow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xbow/refs/heads/main/security/xbow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- Penetration Testing
- Offensive Security
- Artificial Intelligence
- Vulnerability Management
- Cybersecurity
- Application Security
---
