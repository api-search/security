---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: dados.gov.pt
  spf: false
hosts:
- cert_expires: Apr 11 23:59:59 2027 GMT
  host: dados.gov.pt
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Government Portugal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Government, Portugal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Open Government, Portugal
provider_slug: open-government-portugal
slug: open-government-portugal-domain-security
source_filename: open-government-portugal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dados.gov.pt\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dados.gov.pt\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-government-portugal/refs/heads/main/security/open-government-portugal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Government
- Public APIs
---
