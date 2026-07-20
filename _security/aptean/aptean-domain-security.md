---
api_specs:
- filename: aptean-integration-platform-openapi-original.json
  format: json
  label: Aptean Integration Platform API
  slug: aptean-integration-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aptean/refs/heads/main/openapi/aptean-integration-platform-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aptean.com
  spf: true
hosts:
- cert_expires: Oct  8 00:26:37 2026 GMT
  host: www.aptean.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aptean Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aptean, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aptean
provider_slug: aptean
slug: aptean-domain-security
source_filename: aptean-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aptean.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 00:26:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aptean.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aptean/refs/heads/main/security/aptean-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Manufacturing
- ERP
- Supply Chain
- Integration
- Event-Driven
- Webhooks
- Enterprise Software
---
