---
api_specs:
- filename: curai-partner-openapi.json
  format: json
  label: Curai Partner API
  slug: curai-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curai/refs/heads/main/openapi/curai-partner-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: curaihealth.com
  spf: true
hosts:
- cert_expires: Oct 11 16:27:08 2026 GMT
  host: www.curaihealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 23:59:59 2026 GMT
  host: gateway.curaihealth.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Curai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Curai, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Curai
provider_slug: curai
slug: curai-domain-security
source_filename: curai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.curaihealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 16:27:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gateway.curaihealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: curaihealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curai/refs/heads/main/security/curai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- Telemedicine
- Telehealth
- Primary Care
- Digital Health
- Patient Engagement
- Partner API
- SDK
---
