---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: NTT Communications Things Cloud
  slug: things-cloud
  spec_type: OpenAPI
  url: https://developer.ntt.com/iot/docs/reference/openapi/
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: group.ntt
  spf: false
- caa:
  - 0 issue "DigiCert.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: global.ntt
  spf: true
hosts:
- cert_expires: Mar 31 05:31:10 2027 GMT
  host: group.ntt
  hsts: true
  hsts_max_age: 315360000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: www.global.ntt
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.ntt.com
  https: false
kind: domain-security
layout: security
method: probed
name: Ntt Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NTT, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: NTT
provider_slug: ntt-com
slug: ntt-com-domain-security
source_filename: ntt-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: group.ntt\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 31 05:31:10 2027 GMT\n  hsts: true\n  hsts_max_age: 315360000\n- host: www.global.ntt\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.ntt.com\n  https: false\ndomains:\n- domain: group.ntt\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n- domain: global.ntt\n  dnssec: false\n  caa:\n  - 0 issue \"DigiCert.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ntt-com/refs/heads/main/security/ntt-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Telecommunications
- Mobile Networks
- Enterprise Cloud
- Smart Data Platform
- IOWN
- 5G
- IoT
- Things Cloud
- Network APIs
- SD-WAN
- Photonics
- Japan
- Systems Integration
---
