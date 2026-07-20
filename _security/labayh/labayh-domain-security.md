---
api_specs:
- filename: labayh-content-openapi.yml
  format: yaml
  label: Labayh Content API
  slug: content
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/labayh/refs/heads/main/openapi/labayh-content-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: labayh.net
  spf: true
hosts:
- cert_expires: Aug 22 04:36:16 2026 GMT
  host: labayh.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Labayh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Labayh, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Labayh
provider_slug: labayh
slug: labayh-domain-security
source_filename: labayh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: labayh.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 04:36:16 2026 GMT\n  hsts: false\ndomains:\n- domain: labayh.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/labayh/refs/heads/main/security/labayh-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Mental Health
- Healthcare
- Telehealth
- Therapy
- Wellbeing
- Content
- Saudi Arabia
- Middle East
- Arabic
---
