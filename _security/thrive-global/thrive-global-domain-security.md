---
api_specs:
- filename: thrive-global-partner-api-openapi.yml
  format: yaml
  label: Thrive Global Partner API
  slug: thrive-global-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thrive-global/refs/heads/main/openapi/thrive-global-partner-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: thriveglobal.com
  spf: true
hosts:
- cert_expires: Oct 12 21:20:39 2026 GMT
  host: www.thriveglobal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 03:48:25 2026 GMT
  host: partners-api.thriveglobal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 03:48:25 2026 GMT
  host: partners-api-stag.thriveglobal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thrive Global Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thrive Global, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Thrive Global
provider_slug: thrive-global
slug: thrive-global-domain-security
source_filename: thrive-global-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thriveglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 21:20:39 2026 GMT\n  hsts: false\n- host: partners-api.thriveglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:48:25 2026 GMT\n  hsts: null\n- host: partners-api-stag.thriveglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:48:25 2026 GMT\n  hsts: null\ndomains:\n- domain: thriveglobal.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thrive-global/refs/heads/main/security/thrive-global-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Consumer
- Wellness
- Wellbeing
- Behavior Change
- Content
- Healthcare
- Employee Experience
---
