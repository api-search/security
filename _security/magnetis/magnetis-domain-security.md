---
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: true
  domain: magnetis.com.br
  spf: true
hosts:
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: magnetis.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Magnetis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Magnetis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present.'
provider_name: Magnetis
provider_slug: magnetis
slug: magnetis-domain-security
source_filename: magnetis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: magnetis.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: magnetis.com.br\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magnetis/refs/heads/main/security/magnetis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Investing
- Wealth Management
- Robo-Advisor
- Brazil
- Financial Services
---
