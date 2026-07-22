---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: squadio.com
  spf: true
hosts:
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: squadio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Squadio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Squadio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Squadio
provider_slug: squadio
slug: squadio-domain-security
source_filename: squadio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: squadio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: squadio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/squadio/refs/heads/main/security/squadio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Teams as a Service
- Staff Augmentation
- Software Development
- Tech Talent
- Payroll
- MVP Development
- Outsourcing
- MENA
---
