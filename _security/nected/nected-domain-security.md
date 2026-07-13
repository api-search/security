---
api_specs:
- filename: nected-openapi.yml
  format: yaml
  label: Nected
  slug: nected
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nected/refs/heads/main/openapi/nected-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nected.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: nected.io
  spf: true
hosts:
- cert_expires: Sep 16 07:51:49 2026 GMT
  host: www.nected.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: api.nected.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: nected-59.nected.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nected Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nected, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nected
provider_slug: nected
slug: nected-domain-security
source_filename: nected-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nected.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 07:51:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.nected.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: null\n- host: nected-59.nected.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: nected.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: nected.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nected/refs/heads/main/security/nected-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Low-Code
- Workflow Automation
- Decision Engine
- Business Rules
---
