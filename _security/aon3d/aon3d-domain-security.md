---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aon3d.com
  spf: true
hosts:
- cert_expires: Nov 28 06:51:14 2026 GMT
  host: www.aon3d.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 09:12:36 2026 GMT
  host: docs.aon3d.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Aon3D Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AON3D, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AON3D
provider_slug: aon3d
slug: aon3d-domain-security
source_filename: aon3d-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aon3d.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 06:51:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.aon3d.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 18 09:12:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aon3d.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aon3d/refs/heads/main/security/aon3d-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Additive Manufacturing
- 3D Printing
- Industrial Solutions
- Materials
---
