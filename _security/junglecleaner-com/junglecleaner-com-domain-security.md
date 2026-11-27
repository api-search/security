---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: junglecleaner.com
  spf: true
hosts:
- cert_expires: Jan  5 03:19:33 2027 GMT
  host: junglecleaner.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jungle Cleaner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jungle Cleaner, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Jungle Cleaner
provider_slug: junglecleaner-com
slug: junglecleaner-com-domain-security
source_filename: junglecleaner-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: junglecleaner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 03:19:33 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: junglecleaner.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/junglecleaner-com/security/junglecleaner-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Cost Optimization
- Amazon Web Services
- AI Integration
- Free Tier
- Paid Plans
---
