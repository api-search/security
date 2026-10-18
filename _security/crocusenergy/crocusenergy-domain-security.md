---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: crocusenergy.com
  spf: true
hosts:
- cert_expires: Mar 29 21:25:51 2027 GMT
  host: crocusenergy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crocusenergy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crocusenergy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Crocusenergy
provider_slug: crocusenergy
slug: crocusenergy-domain-security
source_filename: crocusenergy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crocusenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 29 21:25:51 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: crocusenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crocusenergy/refs/heads/main/security/crocusenergy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Renewable Energy
- Solar
- Wind
- Cleantech
---
