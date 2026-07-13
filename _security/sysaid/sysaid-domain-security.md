---
api_specs:
- filename: sysaid-openapi.yml
  format: yaml
  label: SysAid REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysaid/refs/heads/main/openapi/sysaid-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sysaid.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: sysaidit.com
  spf: true
hosts:
- cert_expires: Sep 18 22:43:35 2026 GMT
  host: www.sysaid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 07:29:18 2026 GMT
  host: developers.sysaid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: your-account.sysaidit.com
  https: false
kind: domain-security
layout: security
method: probed
name: Sysaid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SysAid, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SysAid
provider_slug: sysaid
slug: sysaid-domain-security
source_filename: sysaid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sysaid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 22:43:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.sysaid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 07:29:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: your-account.sysaidit.com\n  https: false\ndomains:\n- domain: sysaid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: sysaidit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sysaid/refs/heads/main/security/sysaid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ITSM
- Help Desk
- IT Service Management
- Asset Management
- Ticketing
- Service Desk
---
