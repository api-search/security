---
description: ''
domains:
- caa:
  - qsh-idc.caimitech.com.
  dmarc: false
  dnssec: true
  domain: caimitech.com
  spf: true
hosts:
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: caimitech.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Caimitech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for caimitech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: caimitech
provider_slug: caimitech
slug: caimitech-domain-security
source_filename: caimitech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: caimitech.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: caimitech.com\n  dnssec: true\n  caa:\n  - qsh-idc.caimitech.com.\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caimitech/refs/heads/main/security/caimitech-domain-security.yml
summary_line: TLSv1.2 · DNSSEC
tags:
- Company
- FinTech
- Personal Finance
- Wealth Management
- Accounting
- Credit
- Open Platform
- API Gateway
- China
---
