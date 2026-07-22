---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hutchinson.com
  spf: true
hosts:
- cert_expires: Sep  4 11:50:45 2026 GMT
  host: www.hutchinson.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hutchinson Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hutchinson, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hutchinson
provider_slug: hutchinson
slug: hutchinson-domain-security
source_filename: hutchinson-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hutchinson.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 11:50:45 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: hutchinson.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hutchinson/refs/heads/main/security/hutchinson-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automotive
- Tier 1 Supplier
- Anti-Vibration
- Sealing
- Fluid Transfer
- Aerospace
---
