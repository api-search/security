---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fin3000.com
  spf: true
hosts:
- cert_expires: Feb  1 17:04:43 2027 GMT
  host: fin3000.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fin3000 Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fin3000.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fin3000.com
provider_slug: fin3000-com
slug: fin3000-com-domain-security
source_filename: fin3000-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fin3000.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 17:04:43 2027 GMT\n  hsts: null\ndomains:\n- domain: fin3000.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/fin3000-com/security/fin3000-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Accounting
- Invoicing
- E-Invoicing
- XRechnung
- ZUGFeRD
- DATEV
- ELSTER
- Germany
- SaaS
- MCP
---
