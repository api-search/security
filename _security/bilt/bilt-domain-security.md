---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bilt.com
  spf: true
hosts:
- cert_expires: Dec 26 12:52:14 2026 GMT
  host: www.bilt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bilt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BILT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: BILT
provider_slug: bilt
slug: bilt-domain-security
source_filename: bilt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bilt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 12:52:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bilt.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bilt/refs/heads/main/security/bilt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- FinTech
- Loyalty
- Payments
- RentRewards
- CreditCard
- RealEstate
---
