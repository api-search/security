---
api_specs:
- filename: associated-press-meda-openapi-original.yml
  format: yaml
  label: AP Media API
  slug: ap-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/associated-press/refs/heads/main/openapi/associated-press-meda-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ap.org
  spf: true
hosts:
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: www.ap.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: developer.ap.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: api.ap.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Associated Press Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Associated Press, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Associated Press
provider_slug: associated-press
slug: associated-press-domain-security
source_filename: associated-press-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ap.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.ap.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: false\n- host: api.ap.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: ap.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/associated-press/refs/heads/main/security/associated-press-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Elections
- Journalism
- Media
- News
- Content
---
