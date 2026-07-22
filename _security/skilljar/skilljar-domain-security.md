---
api_specs:
- filename: skilljar-openapi-original.yml
  format: yaml
  label: Skilljar API
  slug: skilljar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skilljar/refs/heads/main/openapi/skilljar-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: skilljar.com
  spf: true
hosts:
- cert_expires: Sep 20 00:03:45 2026 GMT
  host: info.skilljar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skilljar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skilljar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Skilljar
provider_slug: skilljar
slug: skilljar-domain-security
source_filename: skilljar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: info.skilljar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 00:03:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: skilljar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skilljar/refs/heads/main/security/skilljar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- Learning Management System
- Customer Education
- Training
- Online Courses
- Certification
- Webhooks
- Enrollment
---
