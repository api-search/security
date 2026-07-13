---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mfapi.in
  spf: false
hosts:
- cert_expires: Sep 11 09:40:36 2026 GMT
  host: www.mfapi.in
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Indian Mutual Fund Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Indian Mutual Fund, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Indian Mutual Fund
provider_slug: indian-mutual-fund
slug: indian-mutual-fund-domain-security
source_filename: indian-mutual-fund-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mfapi.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 09:40:36 2026 GMT\n  hsts: false\ndomains:\n- domain: mfapi.in\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/indian-mutual-fund/refs/heads/main/security/indian-mutual-fund-domain-security.yml
summary_line: TLSv1.3
tags:
- Finance
- Public APIs
---
