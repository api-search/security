---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: false
  dnssec: false
  domain: octaviatech.com
  spf: true
hosts:
- cert_expires: Dec 23 17:43:58 2026 GMT
  host: www.octaviatech.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Octavia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Octavia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Octavia
provider_slug: octavia
slug: octavia-domain-security
source_filename: octavia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.octaviatech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 17:43:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: octaviatech.com\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/octavia/security/octavia-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Exploration
- Critical Minerals
- Geophysics
---
