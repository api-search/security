---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agilemanifesto.org
  spf: false
hosts:
- cert_expires: Sep 29 03:46:19 2026 GMT
  host: agilemanifesto.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agile, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Agile
provider_slug: agile
slug: agile-domain-security
source_filename: agile-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agilemanifesto.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 03:46:19 2026 GMT\n  hsts: false\ndomains:\n- domain: agilemanifesto.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agile/refs/heads/main/security/agile-domain-security.yml
summary_line: TLSv1.3
tags:
- Iterative Development
- Methodology
- Project Management
- Software Development
- Agile Manifesto
- Scrum
- Kanban
---
