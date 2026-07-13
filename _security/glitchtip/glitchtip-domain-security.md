---
api_specs:
- filename: docs
  format: yaml
  label: GlitchTip REST API
  slug: glitchtip-rest-api
  spec_type: OpenAPI
  url: https://app.glitchtip.com/api/docs
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: glitchtip.com
  spf: true
hosts:
- cert_expires: Sep  5 17:24:02 2026 GMT
  host: glitchtip.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 21:32:40 2026 GMT
  host: app.glitchtip.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Glitchtip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GlitchTip, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GlitchTip
provider_slug: glitchtip
slug: glitchtip-domain-security
source_filename: glitchtip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: glitchtip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 17:24:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.glitchtip.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 21:32:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: glitchtip.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glitchtip/refs/heads/main/security/glitchtip-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Error Tracking
- Performance Monitoring
- Uptime Monitoring
- Application Monitoring
- Open Source
- Sentry Compatible
- Observability
- Logging
---
