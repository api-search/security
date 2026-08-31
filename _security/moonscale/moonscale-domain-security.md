---
api_specs:
- filename: moonscale-liveavatar-api-openapi.yml
  format: yaml
  label: Moonscale Live Avatar API
  slug: moonscale-liveavatar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moonscale/refs/heads/main/openapi/moonscale-liveavatar-api-openapi.yml
- filename: moonscale-videogeneration-api-openapi.yml
  format: yaml
  label: Moonscale Video Generation API
  slug: moonscale-videogeneration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moonscale/refs/heads/main/openapi/moonscale-videogeneration-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: moonscale.com
  spf: true
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: mintlify.app
  spf: false
hosts:
- cert_expires: Oct 31 13:05:33 2026 GMT
  host: www.moonscale.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 02:10:29 2026 GMT
  host: vidlab7-d7584a5d.mintlify.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 05:32:51 2026 GMT
  host: api-prd.moonscale.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moonscale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moonscale, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Moonscale
provider_slug: moonscale
slug: moonscale-domain-security
source_filename: moonscale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moonscale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 13:05:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: vidlab7-d7584a5d.mintlify.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 02:10:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-prd.moonscale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 05:32:51 2026 GMT\n  hsts: null\ndomains:\n- domain: moonscale.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mintlify.app\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moonscale/refs/heads/main/security/moonscale-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Sales
- Sales Automation
- Lead Generation
- AI Agents
- Conversational AI
- CRM
- Video Generation
- Avatars
- Speech
- Germany
---
