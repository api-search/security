---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nodejs.org
  spf: true
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: nodejs.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Node Js Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Node.js, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Node.js
provider_slug: node-js
slug: node-js-domain-security
source_filename: node-js-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nodejs.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nodejs.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/node-js/refs/heads/main/security/node-js-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- JavaScript
- Node.js
- Runtime
- Server-Side
---
