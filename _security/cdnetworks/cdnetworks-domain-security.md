---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cdnetworks.com
  spf: true
hosts:
- cert_expires: Nov  9 01:40:44 2026 GMT
  host: cdnetworks.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cdnetworks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CDNetworks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CDNetworks
provider_slug: cdnetworks
slug: cdnetworks-domain-security
source_filename: cdnetworks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cdnetworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 01:40:44 2026 GMT\n  hsts: null\ndomains:\n- domain: cdnetworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cdnetworks/security/cdnetworks-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- CDN
- Cloud Services
- Web Acceleration
- DDoS Protection
- Edge Computing
---
