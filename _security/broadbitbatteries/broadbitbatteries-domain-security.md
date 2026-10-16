---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: broadbit.com
  spf: false
hosts:
- cert_expires: Dec 12 17:55:59 2026 GMT
  host: broadbit.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Broadbitbatteries Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Broadbitbatteries, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Broadbitbatteries
provider_slug: broadbitbatteries
slug: broadbitbatteries-domain-security
source_filename: broadbitbatteries-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: broadbit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 17:55:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: broadbit.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/broadbitbatteries/refs/heads/main/security/broadbitbatteries-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Battery
- Energy
- CleanTech
- Technology
- Finland
---
