---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: krakenshield.eu
  spf: true
hosts:
- cert_expires: Dec 27 15:38:27 2026 GMT
  host: krakenshield.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kraken Shield Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kraken Shield, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kraken Shield
provider_slug: krakenshield-eu
slug: krakenshield-eu-domain-security
source_filename: krakenshield-eu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: krakenshield.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 15:38:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: krakenshield.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/krakenshield-eu/security/krakenshield-eu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cybersecurity
- Audit
- Penetration Testing
- GDPR
- European
---
