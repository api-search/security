---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: erudifi.com
  spf: true
hosts:
- cert_expires: Sep  1 12:47:34 2026 GMT
  host: erudifi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Erudifi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Erudifi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Erudifi
provider_slug: erudifi
slug: erudifi-domain-security
source_filename: erudifi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: erudifi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 12:47:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: erudifi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/erudifi/refs/heads/main/security/erudifi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Education
- Student Financing
- Lending
- Financial Services
- Southeast Asia
---
