---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: autograb.com.au
  spf: true
hosts:
- cert_expires: Dec  4 10:26:58 2026 GMT
  host: autograb.com.au
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Autograb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Autograb, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Autograb
provider_slug: autograb
slug: autograb-domain-security
source_filename: autograb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: autograb.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 10:26:58 2026 GMT\n  hsts: false\ndomains:\n- domain: autograb.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autograb/refs/heads/main/security/autograb-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Automotive
- Data
- Artificial Intelligence
- Marketplace
- Platform
---
