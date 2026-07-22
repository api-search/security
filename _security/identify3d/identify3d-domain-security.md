---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: identify3d.com
  spf: true
hosts:
- cert_expires: Oct  7 00:18:38 2026 GMT
  host: identify3d.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Identify3D Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Identify3D, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Identify3D
provider_slug: identify3d
slug: identify3d-domain-security
source_filename: identify3d-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: identify3d.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 00:18:38 2026 GMT\n  hsts: null\ndomains:\n- domain: identify3d.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/identify3d/refs/heads/main/security/identify3d-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Additive Manufacturing
- 3D Printing
- Digital Manufacturing
- Supply Chain Security
- Digital Rights Management
- Encryption
- Traceability
- Manufacturing
- Acquired
---
