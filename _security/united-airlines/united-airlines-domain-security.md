---
api_specs:
- filename: united-airlines-ndc-openapi.yml
  format: yaml
  label: United Airlines NDC API
  slug: united-airlines-ndc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-airlines/main/openapi/united-airlines-ndc-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: united.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: united.business
  spf: true
hosts:
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: www.united.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 03:51:17 2026 GMT
  host: united.business
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.united.com
  https: false
kind: domain-security
layout: security
method: probed
name: United Airlines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for United Airlines, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: United Airlines
provider_slug: united-airlines
slug: united-airlines-domain-security
source_filename: united-airlines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.united.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: null\n- host: united.business\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 03:51:17 2026 GMT\n  hsts: false\n- host: api.united.com\n  https: false\ndomains:\n- domain: united.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: united.business\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-airlines/refs/heads/main/security/united-airlines-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Airlines
- Travel
- Flight Booking
- NDC
- Loyalty
- Fortune 100
---
