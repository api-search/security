---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ondeck.com
  spf: true
hosts:
- cert_expires: Oct  5 15:58:35 2026 GMT
  host: www.ondeck.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ondeck Capital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OnDeck Capital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: OnDeck Capital
provider_slug: ondeck-capital
slug: ondeck-capital-domain-security
source_filename: ondeck-capital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ondeck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 15:58:35 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: ondeck.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ondeck-capital/refs/heads/main/security/ondeck-capital-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Lending
- Small Business
- Business Loans
- Working Capital
- Financial Services
---
