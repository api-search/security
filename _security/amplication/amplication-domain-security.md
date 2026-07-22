---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: amplication.com
  spf: true
hosts:
- cert_expires: Dec 12 04:38:24 2026 GMT
  host: amplication.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amplication Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amplication, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Amplication
provider_slug: amplication
slug: amplication-domain-security
source_filename: amplication-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amplication.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 04:38:24 2026 GMT\n  hsts: null\ndomains:\n- domain: amplication.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amplication/refs/heads/main/security/amplication-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Backend
- Code Generation
- Developer Tools
- Open Source
- Platform Engineering
- Microservices
- API Development
---
