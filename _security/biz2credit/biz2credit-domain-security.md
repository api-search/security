---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: biz2credit.com
  spf: true
hosts:
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: www.biz2credit.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Biz2Credit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Biz2Credit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Biz2Credit
provider_slug: biz2credit
slug: biz2credit-domain-security
source_filename: biz2credit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.biz2credit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: biz2credit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biz2credit/refs/heads/main/security/biz2credit-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Finance
- Lending
- Small Business
- Online Loans
- Credit
---
