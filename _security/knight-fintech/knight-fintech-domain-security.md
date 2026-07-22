---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: knightfintech.com
  spf: true
hosts:
- cert_expires: Jul 31 23:59:59 2026 GMT
  host: www.knightfintech.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Knight Fintech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Knight Fintech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Knight Fintech
provider_slug: knight-fintech
slug: knight-fintech-domain-security
source_filename: knight-fintech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.knightfintech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 31 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: knightfintech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knight-fintech/refs/heads/main/security/knight-fintech-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Enterprise
- Financial Services
- Banking
- Lending
- Fintech
- Treasury Management
- Embedded Finance
- Supply Chain Finance
- India
---
