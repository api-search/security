---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: js.org
  spf: true
hosts:
- cert_expires: Aug  9 03:03:44 2026 GMT
  host: redux.js.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 20 20:53:45 2026 GMT
  host: react-redux.js.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 14:27:59 2026 GMT
  host: redux-toolkit.js.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Redux Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Redux, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Redux
provider_slug: redux
slug: redux-domain-security
source_filename: redux-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: redux.js.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  9 03:03:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: react-redux.js.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 20 20:53:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: redux-toolkit.js.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 14:27:59 2026 GMT\n  hsts: false\ndomains:\n- domain: js.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/redux/refs/heads/main/security/redux-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Flux Architecture
- Frontend
- Javascript
- Predictable State
- React
- State Management
- Typescript
---
