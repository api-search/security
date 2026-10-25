---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: yancoal.com.au
  spf: true
hosts:
- cert_expires: Jan 15 14:42:54 2027 GMT
  host: yancoal.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Yancoal Australia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yancoal Australia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Yancoal Australia
provider_slug: yancoal-australia
slug: yancoal-australia-domain-security
source_filename: yancoal-australia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yancoal.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 14:42:54 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: yancoal.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yancoal-australia/refs/heads/main/security/yancoal-australia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mining
- Coal
- Energy
- Australia
- Natural Resources
---
