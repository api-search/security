---
api_specs:
- filename: agile-crm-openapi.yml
  format: yaml
  label: Agile CRM REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agile-crm/refs/heads/main/openapi/agile-crm-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agilecrm.com
  spf: true
hosts:
- cert_expires: Oct  2 07:09:18 2026 GMT
  host: www.agilecrm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agile Crm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agile CRM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Agile CRM
provider_slug: agile-crm
slug: agile-crm-domain-security
source_filename: agile-crm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agilecrm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 07:09:18 2026 GMT\n  hsts: false\ndomains:\n- domain: agilecrm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agile-crm/refs/heads/main/security/agile-crm-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- CRM
- Sales Automation
- Marketing Automation
- Helpdesk
- Small Business
- Contact Management
---
