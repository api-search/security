---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: data.gov.sk
  spf: false
hosts:
- cert_expires: Aug 10 22:02:04 2026 GMT
  host: data.gov.sk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Government Slovakia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Government, Slovakia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Open Government, Slovakia
provider_slug: open-government-slovakia
slug: open-government-slovakia-domain-security
source_filename: open-government-slovakia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.gov.sk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 22:02:04 2026 GMT\n  hsts: null\ndomains:\n- domain: data.gov.sk\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-government-slovakia/refs/heads/main/security/open-government-slovakia-domain-security.yml
summary_line: TLSv1.3
tags:
- Government
- Public APIs
---
