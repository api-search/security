---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: keel.so
  spf: false
hosts:
- cert_expires: Oct  4 22:31:35 2026 GMT
  host: keel.so
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Keel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Keel
provider_slug: keel
slug: keel-domain-security
source_filename: keel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: keel.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 22:31:35 2026 GMT\n  hsts: null\ndomains:\n- domain: keel.so\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keel/refs/heads/main/security/keel-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Operations
- ERP
- Backend
- GraphQL
- API
- Low-Code
- Developer Tools
- Workflow
- Authentication
- TypeScript
---
