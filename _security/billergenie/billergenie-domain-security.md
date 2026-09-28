---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: billergenie.com
  spf: true
hosts:
- cert_expires: Dec  9 11:54:00 2026 GMT
  host: merchant.billergenie.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Billergenie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Billergenie, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Billergenie
provider_slug: billergenie
slug: billergenie-domain-security
source_filename: billergenie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: merchant.billergenie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 11:54:00 2026 GMT\n  hsts: null\ndomains:\n- domain: billergenie.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/billergenie/refs/heads/main/security/billergenie-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- SaaS
- Billing
- Payments
- Merchant
- Platform
---
