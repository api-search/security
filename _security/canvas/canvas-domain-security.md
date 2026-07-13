---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: instructure.com
  spf: true
hosts:
- cert_expires: Aug  4 02:52:44 2026 GMT
  host: www.instructure.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: canvas.instructure.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Canvas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Canvas, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Canvas
provider_slug: canvas
slug: canvas-domain-security
source_filename: canvas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.instructure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  4 02:52:44 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: canvas.instructure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: instructure.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canvas/refs/heads/main/security/canvas-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- EdTech
- GraphQL
- Learning Management System
- LMS
- LTI
- Open Source
- REST
---
