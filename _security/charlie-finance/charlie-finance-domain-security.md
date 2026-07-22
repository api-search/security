---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: charlie.com
  spf: true
hosts:
- cert_expires: Oct  2 01:40:53 2026 GMT
  host: charlie.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Charlie Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Charlie Finance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Charlie Finance
provider_slug: charlie-finance
slug: charlie-finance-domain-security
source_filename: charlie-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: charlie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 01:40:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: charlie.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/charlie-finance/refs/heads/main/security/charlie-finance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Banking
- Neobank
- Seniors
- Consumer Finance
- Debit Card
- Social Security
---
