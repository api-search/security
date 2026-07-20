---
api_specs:
- filename: brellium-openapi-original.json
  format: json
  label: Brellium API
  slug: brellium-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/openapi/brellium-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: brellium.com
  spf: true
hosts:
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: api.brellium.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brellium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brellium, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Brellium
provider_slug: brellium
slug: brellium-domain-security
source_filename: brellium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.brellium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: brellium.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/security/brellium-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Clinical Compliance
- Clinical Documentation
- Medical Coding
- Audit
- Behavioral Health
- Digital Health
- API
---
