---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: engiven.com
  spf: true
hosts:
- cert_expires: Feb 11 07:45:21 2027 GMT
  host: engiven.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Engiven Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Engiven, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Engiven
provider_slug: engiven
slug: engiven-domain-security
source_filename: engiven-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: engiven.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 07:45:21 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: engiven.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/engiven/security/engiven-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- NonprofitTech
- CryptoDonations
- Stock Donations
- Enterprise Software
- Financial Compliance
---
