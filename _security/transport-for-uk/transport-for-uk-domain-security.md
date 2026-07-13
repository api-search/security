---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: transportapi.com
  spf: true
hosts:
- cert_expires: Sep 13 08:04:00 2026 GMT
  host: developer.transportapi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Transport For Uk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transport for UK, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Transport for UK
provider_slug: transport-for-uk
slug: transport-for-uk-domain-security
source_filename: transport-for-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.transportapi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 13 08:04:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: transportapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transport-for-uk/refs/heads/main/security/transport-for-uk-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Transportation
- Public APIs
---
