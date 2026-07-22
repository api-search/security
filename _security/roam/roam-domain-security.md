---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: withroam.com
  spf: true
hosts:
- cert_expires: Sep  2 23:46:35 2026 GMT
  host: www.withroam.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Roam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Roam, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Roam
provider_slug: roam
slug: roam-domain-security
source_filename: roam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.withroam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 23:46:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: withroam.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roam/refs/heads/main/security/roam-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Proptech
- Real Estate
- Mortgage
- Assumable Mortgage
- FHA
- VA Loan
- Fintech
- Marketplace
- Home Buying
---
