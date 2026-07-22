---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: american-financial.com
  spf: true
hosts:
- cert_expires: Sep 11 12:10:33 2026 GMT
  host: www.american-financial.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: American Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for American Financial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: American Financial
provider_slug: american-financial
slug: american-financial-domain-security
source_filename: american-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.american-financial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 12:10:33 2026 GMT\n  hsts: null\ndomains:\n- domain: american-financial.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/american-financial/refs/heads/main/security/american-financial-domain-security.yml
summary_line: TLSv1.3
tags:
- Financial Services
- Finance
- Lending
- Fortune 500
---
