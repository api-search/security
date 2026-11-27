---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: immigrationlayer.com
  spf: true
hosts:
- cert_expires: Dec 22 21:35:48 2026 GMT
  host: immigrationlayer.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ImmigrationLayer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ImmigrationLayer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ImmigrationLayer
provider_slug: immigrationlayer-com
slug: immigrationlayer-com-domain-security
source_filename: immigrationlayer-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: immigrationlayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 21:35:48 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: immigrationlayer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/immigrationlayer-com/security/immigrationlayer-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Immigration
- Data API
- USCIS
- Law Firm Tools
---
