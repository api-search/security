---
api_specs:
- filename: toys-r-us-commerce-openapi.yml
  format: yaml
  label: Toys R Us Commerce API
  slug: logicbroker-commerce
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toys-r-us/refs/heads/main/openapi/toys-r-us-commerce-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: toysrus.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: logicbroker.com
  spf: true
hosts:
- cert_expires: Sep  2 16:24:33 2026 GMT
  host: www.toysrus.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 05:58:46 2026 GMT
  host: toysrus.logicbroker.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 30 20:41:45 2026 GMT
  host: commerceapi.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Toys R Us Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Toys R Us, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Toys R Us
provider_slug: toys-r-us
slug: toys-r-us-domain-security
source_filename: toys-r-us-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.toysrus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 16:24:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: toysrus.logicbroker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 05:58:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: commerceapi.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 30 20:41:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: toysrus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: logicbroker.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toys-r-us/refs/heads/main/security/toys-r-us-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Commerce
- Dropship
- E-Commerce
- Retail
- Supply Chain
- Fortune 500
---
