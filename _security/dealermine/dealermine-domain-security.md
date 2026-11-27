---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dealermine.com
  spf: true
hosts:
- cert_expires: Feb  7 17:32:47 2027 GMT
  host: dealermine.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DealerMine Corporation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DealerMine Corporation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DealerMine Corporation
provider_slug: dealermine
slug: dealermine-domain-security
source_filename: dealermine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dealermine.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  7 17:32:47 2027 GMT\n  hsts: null\ndomains:\n- domain: dealermine.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/dealermine/security/dealermine-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Automotive
- Inventory
- B2B
- Marketplace
- Dealer Services
---
