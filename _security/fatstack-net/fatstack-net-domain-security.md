---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fatstack.net
  spf: true
hosts:
- cert_expires: Feb  1 05:30:52 2027 GMT
  host: fatstack.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fatstack Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fatstack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fatstack
provider_slug: fatstack-net
slug: fatstack-net-domain-security
source_filename: fatstack-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fatstack.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 05:30:52 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fatstack.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/fatstack-net/security/fatstack-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Marketplace
- Pay-per-call
- Blockchain
- Tools
---
