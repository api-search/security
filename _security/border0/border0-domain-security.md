---
api_specs:
- filename: border0-openapi.json
  format: json
  label: Border0 API
  slug: border0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/openapi/border0-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: border0.com
  spf: true
hosts:
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: api.border0.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Border0 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Border0, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Border0
provider_slug: border0
slug: border0-domain-security
source_filename: border0-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.border0.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: border0.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/border0/refs/heads/main/security/border0-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Zero Trust
- Network Access
- Security
- Identity and Access Management
- Infrastructure
- VPN
- SSH
- Databases
- Kubernetes
- Company
---
