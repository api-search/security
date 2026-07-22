---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pravica.io
  spf: true
hosts:
- cert_expires: Sep 19 13:16:25 2026 GMT
  host: pravica.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pravica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pravica, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pravica
provider_slug: pravica
slug: pravica-domain-security
source_filename: pravica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pravica.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 13:16:25 2026 GMT\n  hsts: false\ndomains:\n- domain: pravica.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pravica/refs/heads/main/security/pravica-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Financial Services
- Fintech
- Payments
- Programmable Money
- Infrastructure
- Remittances
- Settlement
---
