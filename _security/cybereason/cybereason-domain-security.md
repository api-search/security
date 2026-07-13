---
api_specs:
- filename: cybereason-openapi.yml
  format: yaml
  label: Cybereason REST API
  slug: cybereason-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybereason/refs/heads/main/openapi/cybereason-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cybereason.com
  spf: true
- caa:
  - 0 issue "geotrust.com"
  - 0 issue "globalsign.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cybereason.net
  spf: true
hosts:
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: www.cybereason.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: nest.cybereason.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.cybereason.net
  https: false
kind: domain-security
layout: security
method: probed
name: Cybereason Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cybereason, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cybereason
provider_slug: cybereason
slug: cybereason-domain-security
source_filename: cybereason-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cybereason.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: nest.cybereason.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.cybereason.net\n  https: false\ndomains:\n- domain: cybereason.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: cybereason.net\n  dnssec: false\n  caa:\n  - 0 issue \"geotrust.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cybereason/refs/heads/main/security/cybereason-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cybersecurity
- XDR
- EDR
- NGAV
- MDR
- Endpoint Security
- Threat Detection
---
