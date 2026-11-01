---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chiralnano.com
  spf: true
hosts:
- cert_expires: Nov 28 09:36:40 2026 GMT
  host: www.chiralnano.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chiral Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chiral, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Chiral
provider_slug: chiral
slug: chiral-domain-security
source_filename: chiral-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chiralnano.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 09:36:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: chiralnano.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/chiral/security/chiral-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Semiconductor
- Manufacturing
- Nanomaterials
- Equipment
---
