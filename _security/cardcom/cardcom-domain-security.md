---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cardcom.solutions
  spf: true
hosts:
- cert_expires: Jan 25 18:03:54 2027 GMT
  host: cardcom.solutions
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cardcom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cardcom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Cardcom
provider_slug: cardcom
slug: cardcom-domain-security
source_filename: cardcom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cardcom.solutions\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 18:03:54 2027 GMT\n  hsts: null\ndomains:\n- domain: cardcom.solutions\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/cardcom/security/cardcom-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Payments
- Fintech
- Merchant Services
---
