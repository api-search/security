---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: stake.rent
  spf: true
hosts:
- cert_expires: Dec 14 21:37:12 2026 GMT
  host: stake.rent
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Stake Rent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for @Stake, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: '@Stake'
provider_slug: stake-rent
slug: stake-rent-domain-security
source_filename: stake-rent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stake.rent\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 21:37:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stake.rent\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/stake-rent/security/stake-rent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- FinTech
- CashBack
- Renters
- FinancialServices
---
