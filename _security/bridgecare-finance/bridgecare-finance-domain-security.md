---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getbridgecare.com
  spf: true
hosts:
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: getbridgecare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bridgecare Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BridgeCare Finance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BridgeCare Finance
provider_slug: bridgecare-finance
slug: bridgecare-finance-domain-security
source_filename: bridgecare-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getbridgecare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getbridgecare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bridgecare-finance/refs/heads/main/security/bridgecare-finance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Early Childhood Education
- Child Care
- Government
- GovTech
- Education
- Eligibility & Enrollment
- Grants Management
- Subsidy Management
- SaaS
---
