---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fundingsocieties.com
  spf: true
hosts:
- cert_expires: Sep 22 09:38:51 2026 GMT
  host: fundingsocieties.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Funding Societies Modalku Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Funding Societies | Modalku, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Funding Societies | Modalku
provider_slug: funding-societies-modalku
slug: funding-societies-modalku-domain-security
source_filename: funding-societies-modalku-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fundingsocieties.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 09:38:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fundingsocieties.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/funding-societies-modalku/refs/heads/main/security/funding-societies-modalku-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Financial Services
- Fintech
- SME Lending
- Digital Financing
- Peer-to-Peer Lending
- Invoice Financing
- Investment
- Southeast Asia
---
