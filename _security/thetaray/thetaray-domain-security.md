---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thetaray.com
  spf: true
hosts:
- cert_expires: Oct 19 13:50:20 2026 GMT
  host: thetaray.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 07:29:45 2026 GMT
  host: api.thetaray.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thetaray Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ThetaRay, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ThetaRay
provider_slug: thetaray
slug: thetaray-domain-security
source_filename: thetaray-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thetaray.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 13:50:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.thetaray.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 07:29:45 2026 GMT\n  hsts: null\ndomains:\n- domain: thetaray.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thetaray/refs/heads/main/security/thetaray-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Anti-Money Laundering
- Financial Crime
- Transaction Monitoring
- Sanctions Screening
- KYC
- RegTech
- Risk Assessment
- Artificial Intelligence
- Banking
- Fintech
- Payments
- Compliance
- MCP
---
