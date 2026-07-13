---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: expressjs.com
  spf: false
hosts:
- cert_expires: Aug 22 04:03:06 2026 GMT
  host: expressjs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Express Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Express, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Express
provider_slug: express
slug: express-domain-security
source_filename: express-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: expressjs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 04:03:06 2026 GMT\n  hsts: false\ndomains:\n- domain: expressjs.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/express/refs/heads/main/security/express-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Express.js
- Framework
- HTTP
- Middleware
- Node.js
- Open Source
- Web Framework
- Fortune 1000
---
