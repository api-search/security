---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tetratech.com
  spf: true
hosts:
- cert_expires: Sep 16 10:33:44 2026 GMT
  host: www.tetratech.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 02:32:34 2026 GMT
  host: cosmos.tetratech.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tetra Tech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tetra Tech, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tetra Tech
provider_slug: tetra-tech
slug: tetra-tech-domain-security
source_filename: tetra-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tetratech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 10:33:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cosmos.tetratech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 02:32:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tetratech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tetra-tech/refs/heads/main/security/tetra-tech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Consulting
- Data Management
- Engineering
- Environment
- Infrastructure
- Water
- Fortune 1000
---
