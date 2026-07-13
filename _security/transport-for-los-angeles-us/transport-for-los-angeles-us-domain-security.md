---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: metro.net
  spf: true
hosts:
- cert_expires: Aug 13 23:52:12 2026 GMT
  host: developer.metro.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transport For Los Angeles Us Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transport for Los Angeles, US, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Transport for Los Angeles, US
provider_slug: transport-for-los-angeles-us
slug: transport-for-los-angeles-us-domain-security
source_filename: transport-for-los-angeles-us-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.metro.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 23:52:12 2026 GMT\n  hsts: false\ndomains:\n- domain: metro.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transport-for-los-angeles-us/refs/heads/main/security/transport-for-los-angeles-us-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Transportation
- Public APIs
---
