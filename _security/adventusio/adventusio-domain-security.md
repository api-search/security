---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: adventus.io
  spf: true
hosts:
- cert_expires: Nov 23 02:39:06 2026 GMT
  host: adventus.io
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: api.adventus.io
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Adventusio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adventus.io, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Adventus.io
provider_slug: adventusio
slug: adventusio-domain-security
source_filename: adventusio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adventus.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 23 02:39:06 2026 GMT\n  hsts: false\n- host: api.adventus.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: adventus.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adventusio/refs/heads/main/security/adventusio-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Education
- International Education
- Student Recruitment
- Marketplace
- GraphQL
- Higher Education
- EdTech
- Admissions
- Analytics
---
