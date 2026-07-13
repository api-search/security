---
api_specs:
- filename: drip-openapi.yml
  format: yaml
  label: Drip REST API
  slug: drip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/openapi/drip-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: drip.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getdrip.com
  spf: true
hosts:
- cert_expires: Sep 27 22:06:49 2026 GMT
  host: www.drip.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 07:13:18 2026 GMT
  host: developer.drip.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: api.getdrip.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Drip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Drip, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Drip
provider_slug: drip
slug: drip-domain-security
source_filename: drip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.drip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 22:06:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.drip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 07:13:18 2026 GMT\n  hsts: false\n- host: api.getdrip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: drip.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: getdrip.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drip/refs/heads/main/security/drip-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Marketing
- Marketing Automation
- Ecommerce
- Customer Engagement
- Campaigns
- Workflows
---
