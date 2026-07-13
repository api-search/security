---
api_specs:
- filename: wealthbox-openapi.yml
  format: yaml
  label: Wealthbox CRM API
  slug: crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wealthbox/refs/heads/main/openapi/wealthbox-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wealthbox.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: crmworkspace.com
  spf: true
hosts:
- cert_expires: Oct  1 06:17:51 2026 GMT
  host: www.wealthbox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: dev.wealthbox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 06:29:34 2026 GMT
  host: api.crmworkspace.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wealthbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wealthbox, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wealthbox
provider_slug: wealthbox
slug: wealthbox-domain-security
source_filename: wealthbox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wealthbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 06:17:51 2026 GMT\n  hsts: false\n- host: dev.wealthbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: false\n- host: api.crmworkspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 06:29:34 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: wealthbox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: crmworkspace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wealthbox/refs/heads/main/security/wealthbox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CRM
- Financial Advisors
- Wealth Management
- Contact Management
- Workflow Automation
- SaaS
---
