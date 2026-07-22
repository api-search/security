---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tesorio.com
  spf: true
hosts:
- cert_expires: Sep  7 11:12:56 2026 GMT
  host: www.tesorio.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tesorio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tesorio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tesorio
provider_slug: tesorio
slug: tesorio-domain-security
source_filename: tesorio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tesorio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 11:12:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tesorio.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tesorio/refs/heads/main/security/tesorio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Operations
- Accounts Receivable
- Cash Flow
- Collections
- Treasury
- FinTech
- MCP
---
