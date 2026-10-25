---
api_specs:
- filename: revnu-api-reference-api-openapi.yml
  format: yaml
  label: Revnu API Reference API
  slug: revnu-api-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revnu/refs/heads/main/openapi/revnu-api-reference-api-openapi.yml
- filename: revnu-content-api-api-openapi.yml
  format: yaml
  label: Revnu Content API
  slug: revnu-content-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revnu/refs/heads/main/openapi/revnu-content-api-api-openapi.yml
- filename: revnu-measurement-api-openapi.yml
  format: yaml
  label: Revnu Measurement API
  slug: revnu-measurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revnu/refs/heads/main/openapi/revnu-measurement-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: revnu.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: revnu.app
  spf: true
hosts:
- cert_expires: Dec  6 17:45:52 2026 GMT
  host: revnu.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 20:45:44 2026 GMT
  host: auth.revnu.app
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Revnu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Revnu, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Revnu
provider_slug: revnu
slug: revnu-domain-security
source_filename: revnu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: revnu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 17:45:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: auth.revnu.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 20:45:44 2026 GMT\n  hsts: null\ndomains:\n- domain: revnu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: revnu.app\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revnu/refs/heads/main/security/revnu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Growth Automation
- Marketing
- Artificial Intelligence
- Software-as-a-Service
- Startups
- Lead Generation
- SEO
- MCP
- Agents
- Commerce
- A/B Testing
---
