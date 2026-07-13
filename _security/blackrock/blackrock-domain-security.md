---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: blackrock.com
  spf: true
hosts:
- cert_expires: Aug 27 23:59:59 2026 GMT
  host: www.blackrock.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blackrock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BlackRock, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: BlackRock
provider_slug: blackrock
slug: blackrock-domain-security
source_filename: blackrock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blackrock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blackrock.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blackrock/refs/heads/main/security/blackrock-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Asset Management
- Finance
- FinTech
- Investment Management
- Portfolio Management
- Risk Analytics
- Fortune 500
---
