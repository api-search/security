---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: pcfinancial.ca
  spf: true
hosts:
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: www.pcfinancial.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pc Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PC Financial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: PC Financial
provider_slug: pc-financial
slug: pc-financial-domain-security
source_filename: pc-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pcfinancial.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: pcfinancial.ca\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pc-financial/refs/heads/main/security/pc-financial-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Financial Services
- Banking
- Canada
- Schedule I Bank
- Digital Banking
- Credit Cards
- Loyalty
- Interac
- Data Aggregation
---
