---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: techsoft3d.com
  spf: true
hosts:
- cert_expires: Aug 26 17:43:57 2026 GMT
  host: www.techsoft3d.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tech Soft 3D Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tech Soft 3D, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Tech Soft 3D
provider_slug: tech-soft-3d
slug: tech-soft-3d-domain-security
source_filename: tech-soft-3d-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.techsoft3d.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 17:43:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: techsoft3d.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tech-soft-3d/refs/heads/main/security/tech-soft-3d-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- 3D
- CAD
- SDK
- Visualization
- Data Exchange
- Engineering
- Manufacturing
- Web Components
---
