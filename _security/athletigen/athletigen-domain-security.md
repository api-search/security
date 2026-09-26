---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: athletigen.com
  spf: true
hosts:
- cert_expires: Apr  2 01:13:05 2027 GMT
  host: athletigen.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Athletigen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Athletigen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Athletigen
provider_slug: athletigen
slug: athletigen-domain-security
source_filename: athletigen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: athletigen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  2 01:13:05 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: athletigen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/athletigen/refs/heads/main/security/athletigen-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Health
- Biotechnology
- Genetics
- Wellness
---
