---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: acadio.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: instantdocsbase.com
  spf: false
hosts:
- cert_expires: Dec  2 23:47:31 2026 GMT
  host: acadio.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 02:25:53 2026 GMT
  host: acadio.instantdocsbase.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 07:26:20 2026 GMT
  host: api.acadio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Acadio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acadio, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Acadio
provider_slug: acadio
slug: acadio-domain-security
source_filename: acadio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: acadio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:47:31 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n- host: acadio.instantdocsbase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 02:25:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.acadio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 07:26:20 2026 GMT\n  hsts: null\ndomains:\n- domain: acadio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: instantdocsbase.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acadio/refs/heads/main/security/acadio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- Learning Management System
- Professional Education
- Continuing Education
- Certification
- Exam Preparation
- SCORM
- Webhooks
- Agentic Commerce
---
