---
api_specs:
- filename: tabs-fi-openapi.yml
  format: yaml
  label: Tabs Platform API
  slug: tabs-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabs-fi/refs/heads/main/openapi/tabs-fi-openapi.yml
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
- host: api.tabsplatform.com
  https: false
kind: domain-security
layout: security
method: probed
name: Tabs Fi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tabs, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tabs
provider_slug: tabs-fi
slug: tabs-fi-domain-security
source_filename: tabs-fi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 14:52:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.tabsplatform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 07:01:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tabsplatform.com\n  https: false\ndomains:\n- domain: tabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: tabsplatform.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tabs-fi/refs/heads/main/security/tabs-fi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Tabs
- Revenue
- Billing
- Invoicing
- Accounts Receivable
- Collections
- Revenue Recognition
- Contracts
- Usage
- Payments
- Subscriptions
- Finance
- B2B
---
