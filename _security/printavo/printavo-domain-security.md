---
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issue "pki.goog"
  - 0 issue "globalsign.com"
  - 0 issuewild "globalsign.com"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: printavo.com
  spf: true
hosts:
- cert_expires: Sep  9 22:06:47 2026 GMT
  host: www.printavo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Printavo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Printavo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Printavo
provider_slug: printavo
slug: printavo-domain-security
source_filename: printavo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.printavo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 22:06:47 2026 GMT\n  hsts: false\ndomains:\n- domain: printavo.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/printavo/refs/heads/main/security/printavo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Print Shop Management
- Screen Printing
- Embroidery
- Quotes
- Invoices
- Orders
- GraphQL
- Decorated Apparel
---
