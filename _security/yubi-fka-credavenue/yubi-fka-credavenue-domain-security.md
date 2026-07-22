---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: go-yubi.com
  spf: true
hosts:
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: www.go-yubi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Yubi Fka Credavenue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yubi (fka CredAvenue), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Yubi (fka CredAvenue)
provider_slug: yubi-fka-credavenue
slug: yubi-fka-credavenue-domain-security
source_filename: yubi-fka-credavenue-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.go-yubi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: go-yubi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yubi-fka-credavenue/refs/heads/main/security/yubi-fka-credavenue-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Fintech
- Lending
- Debt Markets
- Co-Lending
- Securitisation
- Supply Chain Finance
- Financial Services
- India
- Credit
---
