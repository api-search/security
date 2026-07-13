---
api_specs:
- filename: sleuth-openapi.yml
  format: yaml
  label: Sleuth Deployments Registration API
  slug: deployments-registration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleuth/refs/heads/main/openapi/sleuth-openapi.yml
- filename: sleuth-openapi.yml
  format: yaml
  label: Sleuth Manual Change API
  slug: manual-change-registration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleuth/refs/heads/main/openapi/sleuth-openapi.yml
- filename: sleuth-openapi.yml
  format: yaml
  label: Sleuth Metric and Incident Impact API
  slug: metric-impact
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleuth/refs/heads/main/openapi/sleuth-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sleuth.io
  spf: true
hosts:
- cert_expires: Aug 23 18:33:50 2026 GMT
  host: www.sleuth.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 10:29:48 2026 GMT
  host: help.sleuth.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: app.sleuth.io
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sleuth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sleuth, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sleuth
provider_slug: sleuth
slug: sleuth-domain-security
source_filename: sleuth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sleuth.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 18:33:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.sleuth.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 10:29:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.sleuth.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\ndomains:\n- domain: sleuth.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sleuth/refs/heads/main/security/sleuth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- DORA
- DevOps
- Deployment Tracking
- Engineering Metrics
- Continuous Delivery
---
