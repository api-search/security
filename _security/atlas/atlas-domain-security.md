---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: theatlas.ai
  spf: false
hosts:
- cert_expires: Oct 11 15:19:01 2026 GMT
  host: theatlas.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atlas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atlas, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Atlas
provider_slug: atlas
slug: atlas-domain-security
source_filename: atlas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: theatlas.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 15:19:01 2026 GMT\n  hsts: false\ndomains:\n- domain: theatlas.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atlas/refs/heads/main/security/atlas-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Artificial Intelligence
- Accounting
- Fintech
- Automation
- Bookkeeping
- Compliance
---
