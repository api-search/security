---
api_specs:
- filename: docs
  format: yaml
  label: Mural Public API
  slug: mural-public-api
  spec_type: Postman
  url: https://developers.mural.co/public/docs
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mural.co
  spf: true
hosts:
- cert_expires: Oct  2 03:59:05 2026 GMT
  host: www.mural.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 18:15:00 2026 GMT
  host: developers.mural.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: app.mural.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mural Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mural, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mural
provider_slug: mural
slug: mural-domain-security
source_filename: mural-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mural.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 03:59:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.mural.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 18:15:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.mural.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mural.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mural/refs/heads/main/security/mural-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Collaboration
- Whiteboard
- Workshops
- Enterprise
- OAuth
---
