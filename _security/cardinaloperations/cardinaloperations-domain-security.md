---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cardopt.com
  spf: false
hosts:
- cert_expires: Nov 11 10:24:06 2026 GMT
  host: cardopt.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cardinaloperations Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cardinaloperations, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Cardinaloperations
provider_slug: cardinaloperations
slug: cardinaloperations-domain-security
source_filename: cardinaloperations-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cardopt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 10:24:06 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: cardopt.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cardinaloperations/refs/heads/main/security/cardinaloperations-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
---
