---
api_specs:
- filename: ribbon-health-h1-api-openapi.yml
  format: yaml
  label: H1 API (Ribbon Health)
  slug: h1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-health/refs/heads/main/openapi/ribbon-health-h1-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: h1.co
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Sep 13 08:52:44 2026 GMT
  host: h1.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: ribbon.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: api.ribbonhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ribbon Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ribbon Health, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ribbon Health
provider_slug: ribbon-health
slug: ribbon-health-domain-security
source_filename: ribbon-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: h1.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 08:52:44 2026 GMT\n  hsts: false\n- host: ribbon.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ribbonhealth.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: h1.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ribbon-health/refs/heads/main/security/ribbon-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Provider Directory
- Insurance
- Clinical Data
- Care Navigation
- Eligibility
- Price Transparency
- Provider Search
- Health Plans
- Digital Health
---
