---
api_specs:
- filename: soothe-help-center-mirror-openapi.json
  format: json
  label: Soothe Help Center Mirror
  slug: soothe-help-center-mirror
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soothe/refs/heads/main/openapi/soothe-help-center-mirror-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: soothe.com
  spf: true
hosts:
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: www.soothe.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 18:04:31 2026 GMT
  host: help.soothe.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Soothe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Soothe, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Soothe
provider_slug: soothe
slug: soothe-domain-security
source_filename: soothe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.soothe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: false\n- host: help.soothe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 18:04:31 2026 GMT\n  hsts: null\ndomains:\n- domain: soothe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soothe/refs/heads/main/security/soothe-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Wellness
- Health and Wellness
- Massage
- Marketplace
- On-Demand Services
- Beauty
- Corporate Wellness
- Hospitality
- Consumer Services
- Local Services
- Booking
---
