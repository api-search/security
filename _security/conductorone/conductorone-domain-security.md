---
api_specs:
- filename: conductorone-openapi-original.yml
  format: yaml
  label: ConductorOne API
  slug: conductorone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conductorone/refs/heads/main/openapi/conductorone-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: conductorone.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: c1.ai
  spf: true
hosts:
- cert_expires: Sep 14 01:03:48 2026 GMT
  host: www.conductorone.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 06:51:34 2026 GMT
  host: www.c1.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: example.conductor.one
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Conductorone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ConductorOne, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ConductorOne
provider_slug: conductorone
slug: conductorone-domain-security
source_filename: conductorone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.conductorone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 01:03:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.c1.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 06:51:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: example.conductor.one\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: conductorone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: c1.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conductorone/refs/heads/main/security/conductorone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cloud Saas
- Identity Security
- Access Governance
- Identity and Access Management
- Access Reviews
- Provisioning
- Least Privilege
- MCP Governance
- Security
---
