---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pfct.co.kr
  spf: true
hosts:
- cert_expires: Dec  9 23:59:59 2026 GMT
  host: pfct.co.kr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Peoplefund Perfect Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PeopleFund, Perfect Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PeopleFund, Perfect Technologies
provider_slug: peoplefund-perfect-technologies
slug: peoplefund-perfect-technologies-domain-security
source_filename: peoplefund-perfect-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pfct.co.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pfct.co.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peoplefund-perfect-technologies/refs/heads/main/security/peoplefund-perfect-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Lending
- Investing
- Artificial Intelligence
- Credit Scoring
- Underwriting
- South Korea
---
