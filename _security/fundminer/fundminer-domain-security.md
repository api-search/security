---
description: ''
domains:
- caa:
  - 0 issuewild "fundminer.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fundminer.com
  spf: true
hosts:
- cert_expires: Sep 13 23:43:44 2026 GMT
  host: fundminer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fundminer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FundMiner, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FundMiner
provider_slug: fundminer
slug: fundminer-domain-security
source_filename: fundminer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fundminer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:43:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fundminer.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"fundminer.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fundminer/refs/heads/main/security/fundminer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fund Management
- Donor Engagement
- Nonprofit
- Higher Education
- Fundraising
- Compliance
- Financial Services
---
