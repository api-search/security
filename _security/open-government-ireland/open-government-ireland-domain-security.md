---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: data.gov.ie
  spf: false
hosts:
- cert_expires: Aug 16 18:40:02 2026 GMT
  host: data.gov.ie
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Government Ireland Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Government, Ireland, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Open Government, Ireland
provider_slug: open-government-ireland
slug: open-government-ireland-domain-security
source_filename: open-government-ireland-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.gov.ie\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 18:40:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: data.gov.ie\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-government-ireland/refs/heads/main/security/open-government-ireland-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Government
- Public APIs
---
