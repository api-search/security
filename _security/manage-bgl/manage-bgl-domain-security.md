---
api_specs:
- filename: manage-bgl-openapi.yml
  format: yaml
  label: Jade Diabetes REST API
  slug: jade-diabetes-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/manage-bgl/refs/heads/main/openapi/manage-bgl-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jadediabetes.com
  spf: true
hosts:
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: jadediabetes.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: app.jadediabetes.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Manage Bgl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Manage BGL, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Manage BGL
provider_slug: manage-bgl
slug: manage-bgl-domain-security
source_filename: manage-bgl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jadediabetes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: false\n- host: app.jadediabetes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jadediabetes.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/manage-bgl/refs/heads/main/security/manage-bgl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Diabetes
- Health
- Healthcare
- Digital Health
- Insulin
- Blood Glucose
- Remote Patient Monitoring
- Telemedicine
- REST API
---
