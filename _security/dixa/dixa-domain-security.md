---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Dixa API
  slug: dixa-api
  spec_type: OpenAPI
  url: https://docs.dixa.io/openapi/dixa-api/beta/overview/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dixa.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dixa.io
  spf: true
hosts:
- cert_expires: Aug 23 10:42:48 2026 GMT
  host: www.dixa.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 00:09:23 2026 GMT
  host: docs.dixa.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 14 23:59:59 2026 GMT
  host: dev.dixa.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dixa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dixa, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dixa
provider_slug: dixa
slug: dixa-domain-security
source_filename: dixa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dixa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 10:42:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.dixa.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 00:09:23 2026 GMT\n  hsts: false\n- host: dev.dixa.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dixa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dixa.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dixa/refs/heads/main/security/dixa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Customer Service
- Conversational
- Omnichannel
- CX
- Help Desk
- Chat
- Knowledge Base
---
