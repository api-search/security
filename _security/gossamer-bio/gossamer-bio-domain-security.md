---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gossamer.co
  spf: false
hosts:
- cert_expires: Jan 12 19:46:02 2027 GMT
  host: gossamer.co
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gossamer Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gossamer Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Gossamer Bio
provider_slug: gossamer-bio
slug: gossamer-bio-domain-security
source_filename: gossamer-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gossamer.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 19:46:02 2027 GMT\n  hsts: null\ndomains:\n- domain: gossamer.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/gossamer-bio/security/gossamer-bio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cannabis
- Edibles
- Beverages
- Pre‑Rolls
- Magazine
- Lifestyle
---
