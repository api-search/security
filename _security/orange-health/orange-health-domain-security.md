---
api_specs:
- filename: orange-health-partner-openapi.yml
  format: yaml
  label: Orange Health Partner API
  slug: orange-health-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-health/refs/heads/main/openapi/orange-health-partner-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 iodef "mailto:secure@orangehealth.in"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: orangehealth.in
  spf: true
- caa:
  - 0 issuewild "amazon.com"
  - 0 iodef "mailto:secure@orangehealth.in"
  - 0 issue "amazon.com"
  dmarc: false
  dnssec: false
  domain: orangehealth.dev
  spf: false
hosts:
- cert_expires: Dec 26 23:59:59 2026 GMT
  host: www.orangehealth.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: partner-api.orangehealth.in
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: sandbox-partner-api.orangehealth.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orange Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orange Health, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Orange Health
provider_slug: orange-health
slug: orange-health-domain-security
source_filename: orange-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.orangehealth.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: partner-api.orangehealth.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: null\n- host: sandbox-partner-api.orangehealth.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: orangehealth.in\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 iodef \"mailto:secure@orangehealth.in\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: orangehealth.dev\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 iodef \"mailto:secure@orangehealth.in\"\n  - 0 issue \"amazon.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orange-health/refs/heads/main/security/orange-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mobile
- Healthcare
- Diagnostics
- Lab Testing
- Home Collection
- Webhooks
- India
---
