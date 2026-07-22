---
api_specs:
- filename: uxcam-data-access-openapi.yml
  format: yaml
  label: UXCam Data Access API
  slug: uxcam-data-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uxcam/refs/heads/main/openapi/uxcam-data-access-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: uxcam.com
  spf: true
hosts:
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: uxcam.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 20:03:55 2026 GMT
  host: developer.uxcam.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: api.uxcam.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uxcam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UXCam, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: UXCam
provider_slug: uxcam
slug: uxcam-domain-security
source_filename: uxcam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uxcam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.uxcam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 20:03:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.uxcam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: uxcam.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uxcam/refs/heads/main/security/uxcam-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Product Analytics
- Session Replay
- Mobile Analytics
- Heatmaps
- User Experience
- Crash Reporting
---
