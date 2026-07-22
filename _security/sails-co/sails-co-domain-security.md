---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sailsjs.com
  spf: true
hosts:
- cert_expires: Aug 27 15:38:45 2026 GMT
  host: sailsjs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sails Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sails Co, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sails Co
provider_slug: sails-co
slug: sails-co-domain-security
source_filename: sails-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sailsjs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 15:38:45 2026 GMT\n  hsts: false\ndomains:\n- domain: sailsjs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sails-co/refs/heads/main/security/sails-co-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Framework
- Node.js
- MVC
- Web Development
- Realtime
- ORM
- REST API
- JavaScript
- Open Source
---
