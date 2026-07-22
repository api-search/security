---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cato.digital
  spf: true
hosts:
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: cato.digital
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: console.cato.digital
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cato Digital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cato Digital, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cato Digital
provider_slug: cato-digital
slug: cato-digital-domain-security
source_filename: cato-digital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cato.digital\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: false\n- host: console.cato.digital\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: cato.digital\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cato-digital/refs/heads/main/security/cato-digital-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cloud
- Bare Metal
- Infrastructure
- GPU
- AI Compute
- Data Center
- Sustainability
- IaaS
- Hosting
- Storage
---
