---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jumo.world
  spf: true
hosts:
- cert_expires: Sep  1 04:43:46 2026 GMT
  host: jumo.world
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jumo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jumo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jumo
provider_slug: jumo
slug: jumo-domain-security
source_filename: jumo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jumo.world\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 04:43:46 2026 GMT\n  hsts: false\ndomains:\n- domain: jumo.world\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jumo/refs/heads/main/security/jumo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Banking as a Service
- Financial Services
- Lending
- Credit
- Mobile Money
- Payments
- Africa
- Emerging Markets
- Artificial Intelligence
---
