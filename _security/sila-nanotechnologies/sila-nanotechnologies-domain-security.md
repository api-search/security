---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: silanano.com
  spf: true
hosts:
- cert_expires: Sep  6 00:25:10 2026 GMT
  host: silanano.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sila Nanotechnologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sila Nanotechnologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sila Nanotechnologies
provider_slug: sila-nanotechnologies
slug: sila-nanotechnologies-domain-security
source_filename: sila-nanotechnologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: silanano.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 00:25:10 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: silanano.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sila-nanotechnologies/refs/heads/main/security/sila-nanotechnologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Battery Materials
- Energy Storage
- Silicon Anode
- Manufacturing
- Advanced Materials
- Clean Energy
---
