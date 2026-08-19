---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: monisnap.com
  spf: true
hosts:
- cert_expires: Oct 19 15:11:06 2026 GMT
  host: www.monisnap.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Monisnap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MONI (Ex-Monisnap), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: MONI (Ex-Monisnap)
provider_slug: monisnap
slug: monisnap-domain-security
source_filename: monisnap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.monisnap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 15:11:06 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: monisnap.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monisnap/refs/heads/main/security/monisnap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech Insurtech
- Money Transfer
- Remittances
- Payments
- Mobile Money
- Airtime Top-Up
- Prepaid Cards
- Embedded Finance
- France
---
