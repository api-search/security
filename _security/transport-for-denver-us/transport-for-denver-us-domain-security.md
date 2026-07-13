---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rtd-denver.com
  spf: true
hosts:
- cert_expires: Aug 30 15:31:26 2026 GMT
  host: www.rtd-denver.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transport For Denver Us Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transport for Denver, US, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Transport for Denver, US
provider_slug: transport-for-denver-us
slug: transport-for-denver-us-domain-security
source_filename: transport-for-denver-us-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rtd-denver.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 15:31:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: rtd-denver.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transport-for-denver-us/refs/heads/main/security/transport-for-denver-us-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Transportation
- Public APIs
---
