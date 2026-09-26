---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: argamedtech.com
  spf: true
hosts:
- cert_expires: Nov 15 10:21:23 2026 GMT
  host: argamedtech.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Argamedtech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Argámedtech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Argámedtech
provider_slug: argamedtech
slug: argamedtech-domain-security
source_filename: argamedtech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: argamedtech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 10:21:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: argamedtech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/argamedtech/refs/heads/main/security/argamedtech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- MedTech
- Cardiology
- Healthcare
- Innovation
---
