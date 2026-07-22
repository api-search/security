---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: samsaraeco.com
  spf: true
hosts:
- cert_expires: Sep  4 23:59:59 2026 GMT
  host: www.samsaraeco.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Samsara Eco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Samsara Eco, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Samsara Eco
provider_slug: samsara-eco
slug: samsara-eco-domain-security
source_filename: samsara-eco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.samsaraeco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: samsaraeco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/samsara-eco/refs/heads/main/security/samsara-eco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Recycling
- Circular Economy
- Biotechnology
- Sustainability
- Materials Science
- Climate Tech
- Plastics
---
