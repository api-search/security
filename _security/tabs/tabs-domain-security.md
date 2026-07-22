---
api_specs:
- filename: tabs-external-api-openapi.yml
  format: yaml
  label: Tabs External API
  slug: tabs-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabs/refs/heads/main/openapi/tabs-external-api-openapi.yml
- filename: tabs-usage-api-beta-openapi.yml
  format: yaml
  label: Tabs Usage API (Beta)
  slug: tabs-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabs/refs/heads/main/openapi/tabs-usage-api-beta-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tabs.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tabsplatform.com
  spf: true
hosts:
- cert_expires: Sep 19 14:52:03 2026 GMT
  host: www.tabs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 07:01:43 2026 GMT
  host: docs.tabsplatform.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: integrators.prod.api.tabsplatform.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tabs, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tabs
provider_slug: tabs
slug: tabs-domain-security
source_filename: tabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 14:52:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.tabsplatform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 07:01:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: integrators.prod.api.tabsplatform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: tabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: tabsplatform.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tabs/refs/heads/main/security/tabs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Billing
- Revenue Automation
- Accounts Receivable
- Revenue Recognition
- Usage-Based Billing
- Invoicing
- Collections
- Fintech
- SaaS
---
