---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: smics.com
  spf: true
hosts:
- cert_expires: Jan 10 02:39:37 2027 GMT
  host: www.smics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Semiconductor Manufacturing International Corporation Smic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Semiconductor Manufacturing International Corporation (SMIC), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Semiconductor Manufacturing International Corporation (SMIC)
provider_slug: semiconductor-manufacturing-international-corporation-smic
slug: semiconductor-manufacturing-international-corporation-smic-domain-security
source_filename: semiconductor-manufacturing-international-corporation-smic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.smics.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 10 02:39:37 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: smics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/semiconductor-manufacturing-international-corporation-smic/security/semiconductor-manufacturing-international-corporation-smic-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Semiconductor
- Foundry
- China
- Manufacturing
- Technology
---
