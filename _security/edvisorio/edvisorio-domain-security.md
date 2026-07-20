---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: edvisor.io
  spf: true
hosts:
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: edvisor.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Edvisorio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Edvisor.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Edvisor.io
provider_slug: edvisorio
slug: edvisorio-domain-security
source_filename: edvisorio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: edvisor.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: edvisor.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edvisorio/refs/heads/main/security/edvisorio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Education
- Student Recruitment
- International Education
- EdTech
- GraphQL
- Marketplace
- Webhooks
---
