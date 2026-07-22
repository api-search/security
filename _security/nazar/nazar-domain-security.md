---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nazar.ai
  spf: true
hosts:
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: nazar.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nazar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nazar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Nazar
provider_slug: nazar
slug: nazar-domain-security
source_filename: nazar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nazar.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: nazar.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nazar/refs/heads/main/security/nazar-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Database
- Database Monitoring
- Performance
- Observability
- Cost Optimization
- SQL
- Artificial Intelligence
- DevOps
---
