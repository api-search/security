---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Tryton REST API
  slug: tryton-rest-api
  spec_type: OpenAPI
  url: https://docs.tryton.org/latest/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tryton.org
  spf: true
hosts:
- cert_expires: Sep 26 00:27:49 2026 GMT
  host: www.tryton.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 20:36:25 2026 GMT
  host: discuss.tryton.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tryton Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tryton, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tryton
provider_slug: tryton
slug: tryton-domain-security
source_filename: tryton-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tryton.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 00:27:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: discuss.tryton.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 20:36:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tryton.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tryton/refs/heads/main/security/tryton-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ERP
- Enterprise Resource Planning
- Accounting
- Inventory
- Sales
- Purchasing
- Production
- Project Management
- Open Source
---
