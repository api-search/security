---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: iprate.eu
  spf: true
hosts:
- cert_expires: Dec 22 02:57:46 2026 GMT
  host: iprate.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: IPRATE Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IPRATE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: IPRATE
provider_slug: iprate-eu
slug: iprate-eu-domain-security
source_filename: iprate-eu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iprate.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 02:57:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: iprate.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/iprate-eu/security/iprate-eu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- IP
- Ratings
- Europe
- Data
---
