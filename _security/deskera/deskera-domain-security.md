---
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "ssl.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: deskera.com
  spf: true
hosts:
- cert_expires: Sep 30 19:22:17 2026 GMT
  host: www.deskera.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: bifrost-us.deskera.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deskera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deskera, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Deskera
provider_slug: deskera
slug: deskera-domain-security
source_filename: deskera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.deskera.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 30 19:22:17 2026 GMT\n  hsts: null\n- host: bifrost-us.deskera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: deskera.com\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deskera/refs/heads/main/security/deskera-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- ERP
- Accounting
- CRM
- Human Resources
- Payroll
- Inventory
- Invoicing
- Small Business
- Software-as-a-Service
---
