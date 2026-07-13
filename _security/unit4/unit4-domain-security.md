---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: unit4.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: unit4rd.com
  spf: false
hosts:
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: www.unit4.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: develop.unit4rd.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.unit4.com
  https: false
kind: domain-security
layout: security
method: probed
name: Unit4 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unit4, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Unit4
provider_slug: unit4
slug: unit4-domain-security
source_filename: unit4-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unit4.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: null\n- host: develop.unit4rd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: false\n- host: api.unit4.com\n  https: false\ndomains:\n- domain: unit4.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: unit4rd.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unit4/refs/heads/main/security/unit4-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- ERP
- Cloud ERP
- Enterprise Resource Planning
- Financials
- Human Resources
- Payroll
- Project Management
- Procurement
- Inventory Management
- Business Planning
- PEPPOL
- E-Invoicing
- Service Organizations
- Public Sector
---
