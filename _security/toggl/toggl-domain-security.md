---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: toggl.com
  spf: true
hosts:
- cert_expires: Aug 28 04:25:48 2026 GMT
  host: toggl.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 04:52:39 2026 GMT
  host: engineering.toggl.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 07:46:20 2026 GMT
  host: api.track.toggl.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Toggl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Toggl Track, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Toggl Track
provider_slug: toggl
slug: toggl-domain-security
source_filename: toggl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: toggl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 04:25:48 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: engineering.toggl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 04:52:39 2026 GMT\n  hsts: false\n- host: api.track.toggl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 07:46:20 2026 GMT\n  hsts: null\ndomains:\n- domain: toggl.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toggl/refs/heads/main/security/toggl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Time Tracking
- Productivity
- Project Management
- Billing
- Reporting
- Workforce Management
---
