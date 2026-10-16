---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jawbone.com
  spf: true
hosts:
- cert_expires: Jan  2 18:20:43 2027 GMT
  host: www.jawbone.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jawbone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jawbone, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Jawbone
provider_slug: jawbone
slug: jawbone-domain-security
source_filename: jawbone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jawbone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 18:20:43 2027 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: jawbone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jawbone/refs/heads/main/security/jawbone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Wearables
- Consumer Electronics
- Health Tech
- Bluetooth
---
