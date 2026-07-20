---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: butterpayments.com
  spf: true
hosts:
- cert_expires: Oct  4 00:54:13 2026 GMT
  host: butterpayments.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Butterpayments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Butterpayments, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Butterpayments
provider_slug: butterpayments
slug: butterpayments-domain-security
source_filename: butterpayments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: butterpayments.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  4 00:54:13 2026 GMT\n  hsts: false\ndomains:\n- domain: butterpayments.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/butterpayments/refs/heads/main/security/butterpayments-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Company
- Payments
- Payment Recovery
- Subscriptions
- Dunning
- Involuntary Churn
- Dispute Prevention
- Chargebacks
- Card Vault
- Fintech
- Machine Learning
---
