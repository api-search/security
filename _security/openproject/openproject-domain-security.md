---
api_specs:
- filename: openproject-openapi.yml
  format: yaml
  label: OpenProject API v3
  slug: openproject-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openproject/refs/heads/main/openapi/openproject-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: openproject.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: openproject-edge.com
  spf: true
hosts:
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: www.openproject.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: community.openproject.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: qa.openproject-edge.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openproject Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenProject, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OpenProject
provider_slug: openproject
slug: openproject-domain-security
source_filename: openproject-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openproject.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: community.openproject.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: qa.openproject-edge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: openproject.org\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: openproject-edge.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openproject/refs/heads/main/security/openproject-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Agile
- Gantt
- Open Source
- Project Management
- Time Tracking
- Work Packages
---
