---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: divine.inc
  spf: true
hosts:
- cert_expires: Aug 24 05:14:50 2026 GMT
  host: divine.inc
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Divine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Divine, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Divine
provider_slug: divine
slug: divine-domain-security
source_filename: divine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: divine.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 05:14:50 2026 GMT\n  hsts: false\ndomains:\n- domain: divine.inc\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/divine/refs/heads/main/security/divine-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Crypto
- Fintech
- Lending
- Stablecoins
- DeFi
- Credit
---
