---
api_specs:
- filename: reonic-openapi-original.json
  format: json
  label: Reonic REST API v3
  slug: reonic-rest-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reonic/refs/heads/main/openapi/reonic-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: reonic.de
  spf: true
hosts:
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: reonic.de
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reonic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reonic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Reonic
provider_slug: reonic
slug: reonic-domain-security
source_filename: reonic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reonic.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: reonic.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reonic/refs/heads/main/security/reonic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Climate Energy
- Solar
- Renewable Energy
- Photovoltaic
- Heat Pumps
- Installer Software
- SaaS
- CRM
- Project Management
---
