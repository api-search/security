---
api_specs:
- filename: swagger.json
  format: json
  label: Everbridge Suite API
  slug: everbridge-suite-api
  spec_type: OpenAPI
  url: https://api.everbridge.net/rest/swagger.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: everbridge.net
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: everbridge.com
  spf: true
hosts:
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: manager.everbridge.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: www.everbridge.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 01:48:29 2026 GMT
  host: developers.everbridge.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Everbridge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Everbridge, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Everbridge
provider_slug: everbridge
slug: everbridge-domain-security
source_filename: everbridge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: manager.everbridge.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.everbridge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.everbridge.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 01:48:29 2026 GMT\n  hsts: null\ndomains:\n- domain: everbridge.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: everbridge.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/everbridge/refs/heads/main/security/everbridge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Critical Event Management
- Emergency Management
- Incident Management
- IT Alerting
- Mass Notification
---
