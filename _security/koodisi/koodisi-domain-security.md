---
api_specs:
- filename: koodisi-openapi-generated.yml
  format: yaml
  label: Ivoyant API
  slug: koodisi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koodisi/refs/heads/main/openapi/_ae-authored/koodisi-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: koodisi.com
  spf: true
hosts:
- cert_expires: Jan  3 05:39:22 2027 GMT
  host: koodisi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Koodisi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ivoyant, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ivoyant
provider_slug: koodisi
slug: koodisi-domain-security
source_filename: koodisi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: koodisi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 05:39:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: koodisi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koodisi/refs/heads/main/security/koodisi-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Integration Platform
- iPaaS
- Workflow Automation
- Enterprise Integration
- API Management
- Governance
- AI Agents
- Multi‑tenant
---
