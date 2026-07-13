---
api_specs:
- filename: intercom-openapi.yml
  format: yaml
  label: Intercom API
  slug: intercom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intercom/refs/heads/main/openapi/intercom-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: intercom.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: intercom.io
  spf: true
hosts:
- cert_expires: Oct  8 15:01:37 2026 GMT
  host: developers.intercom.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: www.intercom.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: api.intercom.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Intercom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intercom, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Intercom
provider_slug: intercom
slug: intercom-domain-security
source_filename: intercom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.intercom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 15:01:37 2026 GMT\n  hsts: false\n- host: www.intercom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.intercom.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: intercom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: intercom.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intercom/refs/heads/main/security/intercom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Customer Service
- Customer Support
- Messaging
---
