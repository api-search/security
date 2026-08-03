---
api_specs:
- filename: intelycare-external-scheduling-openapi.yml
  format: yaml
  label: IntelyCare External Scheduling API
  slug: intelycare-external-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/intelycare/refs/heads/main/openapi/intelycare-external-scheduling-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: intelycare.com
  spf: true
hosts:
- cert_expires: Oct  9 13:08:10 2026 GMT
  host: www.intelycare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 15:24:19 2026 GMT
  host: apidocs.intelycare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: api.intelycare.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Intelycare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IntelyCare, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: IntelyCare
provider_slug: intelycare
slug: intelycare-domain-security
source_filename: intelycare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.intelycare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:08:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.intelycare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 15:24:19 2026 GMT\n  hsts: false\n- host: api.intelycare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: intelycare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intelycare/refs/heads/main/security/intelycare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- healthcare
- healthcare-staffing
- nursing
- workforce-management
- scheduling
- shift-management
- timekeeping
- marketplace
- webhooks
- per-diem
- credentialing
- post-acute-care
---
