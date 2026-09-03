---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: formboost.app
  spf: true
hosts:
- cert_expires: Nov 19 13:46:41 2026 GMT
  host: formboost.app
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Formboost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Formboost, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Formboost
provider_slug: formboost
slug: formboost-domain-security
source_filename: formboost-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: formboost.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 13:46:41 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: formboost.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/formboost/refs/heads/main/security/formboost-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- forms
- form-backend
- html-forms
- serverless
- static-sites
- react
- nextjs
- vue
- webhooks
- no-code
- developer-tools
- spam-filtering
---
