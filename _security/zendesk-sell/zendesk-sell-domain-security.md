---
api_specs:
- filename: zendesk-sell-openapi.yml
  format: yaml
  label: Zendesk Sell (Sales CRM) API
  slug: sales-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zendesk-sell/refs/heads/main/openapi/zendesk-sell-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zendesk.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getbase.com
  spf: true
hosts:
- cert_expires: Oct  5 12:14:30 2026 GMT
  host: www.zendesk.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 01:00:41 2026 GMT
  host: developer.zendesk.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 22:32:56 2026 GMT
  host: api.getbase.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zendesk Sell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zendesk Sell, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zendesk Sell
provider_slug: zendesk-sell
slug: zendesk-sell-domain-security
source_filename: zendesk-sell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zendesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 12:14:30 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: developer.zendesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 01:00:41 2026 GMT\n  hsts: false\n- host: api.getbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 22:32:56 2026 GMT\n  hsts: null\ndomains:\n- domain: zendesk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: getbase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zendesk-sell/refs/heads/main/security/zendesk-sell-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CRM
- Sales
- Sales Automation
- Leads
- Deals
- Pipeline
- Customer Experience
---
