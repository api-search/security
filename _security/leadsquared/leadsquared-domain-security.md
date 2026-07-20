---
api_specs:
- filename: postman.yaml
  format: yaml
  label: LeadSquared REST API
  slug: rest-api
  spec_type: Postman
  url: https://apidocs.leadsquared.com/leadsquared-run-in-postman/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: leadsquared.com
  spf: true
hosts:
- cert_expires: Aug 15 02:05:01 2026 GMT
  host: www.leadsquared.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 08:45:45 2026 GMT
  host: apidocs.leadsquared.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: api.leadsquared.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leadsquared Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LeadSquared, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LeadSquared
provider_slug: leadsquared
slug: leadsquared-domain-security
source_filename: leadsquared-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.leadsquared.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 02:05:01 2026 GMT\n  hsts: false\n- host: apidocs.leadsquared.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 08:45:45 2026 GMT\n  hsts: false\n- host: api.leadsquared.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: leadsquared.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leadsquared/refs/heads/main/security/leadsquared-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Marketing Automation
- CRM
- Sales Automation
- Lead Management
- Customer Engagement
- Field Force Automation
---
