---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: docquity.com
  spf: true
hosts:
- cert_expires: Dec 16 15:22:41 2026 GMT
  host: docquity.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  role: website
  tls_version: TLSv1.3
- cert_expires: Dec 16 15:22:41 2026 GMT
  host: api.docquity.com
  hsts: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  note: not discovered from apis.yml (no public API entry); probed directly
  role: first-party application backend
  tls_version: TLSv1.3
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: app.docquity.com
  hsts: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  role: web application
  tls_version: TLSv1.3
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: id.docquity.com
  hsts: true
  hsts_max_age: 31536000
  hsts_preload: false
  https: true
  note: Returns 401 on every path including /.well-known/openid-configuration. Negotiates TLS 1.2 where every other Docquity host negotiates TLS 1.3.
  role: identity service
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Docquity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Docquity, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Docquity
provider_slug: docquity
slug: docquity-domain-security
source_filename: docquity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docquity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 15:22:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  role: website\n- host: api.docquity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 15:22:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_preload: true\n  role: first-party application backend\n  note: not discovered from apis.yml (no public API entry); probed directly\n- host: app.docquity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_preload: true\n  role: web application\n- host: id.docquity.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_preload: false\n  role: identity service\n  note: >-\n    Returns 401 on every path\
  \ including /.well-known/openid-configuration.\n    Negotiates TLS 1.2 where every other Docquity host negotiates TLS 1.3.\ndomains:\n- domain: docquity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docquity/refs/heads/main/security/docquity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Digital Health
- Medical Education
- Healthcare Professionals
- Professional Network
- Life Sciences
- Pharmaceuticals
- Artificial Intelligence
- Clinical Decision Support
- Mobile
- Southeast Asia
- Singapore
---
