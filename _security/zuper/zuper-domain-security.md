---
api_specs:
- filename: llms.txt
  format: yaml
  label: Zuper REST API
  slug: zuper-rest-api
  spec_type: OpenAPI
  url: https://developers.zuper.co/llms.txt
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zuper.co
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zuperpro.com
  spf: false
hosts:
- cert_expires: Aug 14 08:02:50 2026 GMT
  host: www.zuper.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 01:28:31 2026 GMT
  host: developers.zuper.co
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 08:31:37 2026 GMT
  host: accounts.zuperpro.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zuper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zuper, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Zuper
provider_slug: zuper
slug: zuper-domain-security
source_filename: zuper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zuper.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 08:02:50 2026 GMT\n  hsts: false\n- host: developers.zuper.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 01:28:31 2026 GMT\n  hsts: null\n- host: accounts.zuperpro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 08:31:37 2026 GMT\n  hsts: false\ndomains:\n- domain: zuper.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: zuperpro.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zuper/refs/heads/main/security/zuper-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Field Service Management
- Scheduling
- Dispatching
- Invoicing
- Timesheets
- Asset Management
- Work Orders
- Customer Management
- Inventory
- Projects
---
