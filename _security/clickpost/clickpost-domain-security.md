---
api_specs:
- filename: clickpost-openapi.yml
  format: yaml
  label: ClickPost API
  slug: clickpost-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickpost/refs/heads/main/openapi/clickpost-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: clickpost.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clickpost.in
  spf: true
hosts:
- cert_expires: Aug 24 11:41:22 2026 GMT
  host: www.clickpost.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 07:54:43 2026 GMT
  host: docs.clickpost.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: www.clickpost.in
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Clickpost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClickPost, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: ClickPost
provider_slug: clickpost
slug: clickpost-domain-security
source_filename: clickpost-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clickpost.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 11:41:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.clickpost.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 07:54:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.clickpost.in\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: clickpost.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: clickpost.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clickpost/refs/heads/main/security/clickpost-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Carriers
- Delivery
- E-Commerce Logistics
- Logistics
- Returns
- Shipping
- Supply Chain
- Tracking
---
