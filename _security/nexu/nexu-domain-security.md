---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nexu.mx
  spf: true
hosts:
- cert_expires: Oct 21 00:08:21 2026 GMT
  host: www.nexu.mx
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nexu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nexu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nexu
provider_slug: nexu
slug: nexu-domain-security
source_filename: nexu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nexu.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 00:08:21 2026 GMT\n  hsts: false\ndomains:\n- domain: nexu.mx\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexu/refs/heads/main/security/nexu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Financial-Services
- Fintech
- Lending
- Auto Finance
- Leasing
- Automotive
- Consumer Credit
- Mexico
---
