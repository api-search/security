---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hkam-group.com
  spf: true
hosts:
- cert_expires: Oct  2 15:33:20 2026 GMT
  host: hkam-group.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Hong Kong Asia Medical Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hong Kong Asia Medical Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Hong Kong Asia Medical Group
provider_slug: hong-kong-asia-medical-group
slug: hong-kong-asia-medical-group-domain-security
source_filename: hong-kong-asia-medical-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hkam-group.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  2 15:33:20 2026 GMT\n  hsts: false\ndomains:\n- domain: hkam-group.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hong-kong-asia-medical-group/refs/heads/main/security/hong-kong-asia-medical-group-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Healthcare
- Hospital
- Cardiovascular
- Medical
- Asia
- Hong Kong
---
