---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hilltop.com
  spf: true
hosts:
- cert_expires: Nov  1 15:04:03 2026 GMT
  host: www.hilltop.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hilltop Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hilltop Holdings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hilltop Holdings
provider_slug: hilltop-holdings
slug: hilltop-holdings-domain-security
source_filename: hilltop-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hilltop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 15:04:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hilltop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hilltop-holdings/refs/heads/main/security/hilltop-holdings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Insurance
- Financial-Services
- Mortgage
- Broker-Dealer
- Wealth Management
- Holding Company
---
