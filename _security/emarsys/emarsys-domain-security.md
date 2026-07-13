---
api_specs:
- filename: emarsys-openapi.yml
  format: yaml
  label: SAP Emarsys Core API
  slug: core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emarsys/refs/heads/main/openapi/emarsys-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: emarsys.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: emarsys.net
  spf: true
hosts:
- cert_expires: Aug 18 05:49:44 2026 GMT
  host: emarsys.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 12:34:03 2026 GMT
  host: dev.emarsys.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: api.emarsys.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Emarsys Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SAP Emarsys, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SAP Emarsys
provider_slug: emarsys
slug: emarsys-domain-security
source_filename: emarsys-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: emarsys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 05:49:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.emarsys.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 12:34:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.emarsys.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: emarsys.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: emarsys.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emarsys/refs/heads/main/security/emarsys-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketing Automation
- Customer Engagement
- Email Marketing
- Omnichannel
- Customer Data Platform
- SAP
---
