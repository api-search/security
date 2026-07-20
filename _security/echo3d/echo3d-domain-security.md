---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: echo3d.com
  spf: true
hosts:
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: www.echo3d.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 20:57:54 2026 GMT
  host: docs.echo3d.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: api.echo3d.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Echo3D Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for echo3D, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: echo3D
provider_slug: echo3d
slug: echo3d-domain-security
source_filename: echo3d-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.echo3d.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: false\n- host: docs.echo3d.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 20:57:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.echo3d.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: echo3d.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/echo3d/refs/heads/main/security/echo3d-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- 3D
- Augmented Reality
- Virtual Reality
- Digital Asset Management
- 3D Models
- Content Delivery
- Developer Tools
- SDKs
- WebAR
---
