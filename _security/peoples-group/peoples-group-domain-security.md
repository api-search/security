---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: peoplesgroup.com
  spf: true
hosts:
- cert_expires: Sep 30 17:14:06 2026 GMT
  host: www.peoplesgroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Peoples Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Peoples Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Peoples Group
provider_slug: peoples-group
slug: peoples-group-domain-security
source_filename: peoples-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.peoplesgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 17:14:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: peoplesgroup.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peoples-group/refs/heads/main/security/peoples-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Payments
- Canada
- Banking as a Service
- Card Issuing
- Money Movement
- Interac e-Transfer
- EFT
- Bill Payments
- Merchant Acquiring
- Real-Time Payments
- ISO 20022
- BIN Sponsorship
---
