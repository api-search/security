---
api_specs:
- filename: sedna-openapi.json
  format: json
  label: Sedna API
  slug: sedna-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sedna.com
  spf: true
hosts:
- cert_expires: Oct  1 05:47:40 2026 GMT
  host: sedna.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sedna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SEDNA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SEDNA
provider_slug: sedna
slug: sedna-domain-security
source_filename: sedna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sedna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 05:47:40 2026 GMT\n  hsts: false\ndomains:\n- domain: sedna.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/security/sedna-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Shipping
- Maritime
- Email
- Communications
- Workflow
- Commodity Trading
- Logistics
- Messaging
---
