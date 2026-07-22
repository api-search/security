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
- cert_expires: Sep  9 10:07:06 2026 GMT
  host: www.bilt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bilt Rewards Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bilt Rewards, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bilt Rewards
provider_slug: bilt-rewards
slug: bilt-rewards-domain-security
source_filename: bilt-rewards-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bilt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 10:07:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bilt.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bilt-rewards/refs/heads/main/security/bilt-rewards-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Rewards
- Loyalty
- Payments
- Rent
- Mortgage
- Credit Cards
- Membership
---
