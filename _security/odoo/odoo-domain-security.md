---
api_specs:
- filename: odoo-openapi.yml
  format: yaml
  label: Odoo External API
  slug: odoo-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/odoo/refs/heads/main/openapi/odoo-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:abuse@odoo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: odoo.com
  spf: true
hosts:
- cert_expires: Aug 26 18:28:20 2026 GMT
  host: www.odoo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Odoo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Odoo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Odoo
provider_slug: odoo
slug: odoo-domain-security
source_filename: odoo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.odoo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 18:28:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: odoo.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:abuse@odoo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/odoo/refs/heads/main/security/odoo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business Applications
- CRM
- ERP
- Open Source
---
