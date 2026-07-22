---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: moradocolombia.com
  spf: false
hosts:
- cert_expires: Sep  6 09:11:45 2026 GMT
  host: www.moradocolombia.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Morado Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Morado, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Morado
provider_slug: morado
slug: morado-domain-security
source_filename: morado-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moradocolombia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 09:11:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: moradocolombia.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/morado/refs/heads/main/security/morado-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Marketplace
- Fintech
- Beauty
- Wellness
- Lending
- Credit
- Colombia
- Latin America
- B2B
---
