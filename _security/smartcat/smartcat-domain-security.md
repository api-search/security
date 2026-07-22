---
api_specs:
- filename: smartcat-openapi.json
  format: json
  label: Smartcat API v1
  slug: smartcat-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartcat/refs/heads/main/openapi/smartcat-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: smartcat.com
  spf: true
hosts:
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: smartcat.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smartcat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smartcat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Smartcat
provider_slug: smartcat
slug: smartcat-domain-security
source_filename: smartcat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smartcat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: smartcat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartcat/refs/heads/main/security/smartcat-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai
- Translation
- Localization
- Language
- Machine Translation
- Content
- Translation Management
---
