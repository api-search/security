---
api_specs:
- filename: adlumininc-api-openapi-original.yml
  format: yaml
  label: Adlumin XDR/MDR API
  slug: adlumin-xdrmdr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adlumininc/refs/heads/main/openapi/adlumininc-api-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: n-able.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adlumin.com
  spf: true
hosts:
- cert_expires: Nov  4 03:20:55 2026 GMT
  host: www.n-able.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 23:00:36 2026 GMT
  host: developer.n-able.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: api.adlumin.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Adlumininc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adlumin, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Adlumin
provider_slug: adlumininc
slug: adlumininc-domain-security
source_filename: adlumininc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.n-able.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 03:20:55 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: developer.n-able.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:00:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.adlumin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: n-able.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: adlumin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adlumininc/refs/heads/main/security/adlumininc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Security
- Cybersecurity
- Managed Detection and Response
- Extended Detection and Response
- SIEM
- SOAR
- Threat Detection
- Endpoint Security
- Compliance
- Managed Service Providers
- MCP
- agent-native
---
