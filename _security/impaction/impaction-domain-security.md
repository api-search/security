---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: impaction.team
  spf: true
hosts:
- cert_expires: Dec 11 22:52:41 2026 GMT
  host: impaction.team
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Impaction Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Impaction, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Impaction
provider_slug: impaction
slug: impaction-domain-security
source_filename: impaction-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: impaction.team\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 22:52:41 2026 GMT\n  hsts: false\ndomains:\n- domain: impaction.team\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/impaction/refs/heads/main/security/impaction-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Consulting
- Agile
- DigitalTransformation
- Leadership
---
