---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bigbelly.com
  spf: true
hosts:
- cert_expires: Jan 18 00:24:31 2027 GMT
  host: bigbelly.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bigbelly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bigbelly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bigbelly
provider_slug: bigbelly
slug: bigbelly-domain-security
source_filename: bigbelly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bigbelly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 00:24:31 2027 GMT\n  hsts: false\ndomains:\n- domain: bigbelly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/bigbelly/security/bigbelly-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Waste Management
- Smart Bins
- Public Space
- Municipal Solutions
- Recycling
- Compost
- Software
---
