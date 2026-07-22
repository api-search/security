---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: claimglide.com
  spf: true
hosts:
- cert_expires: Jan  2 21:19:18 2027 GMT
  host: claimglide.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Claimglide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Claimglide, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Claimglide
provider_slug: claimglide
slug: claimglide-domain-security
source_filename: claimglide-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: claimglide.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  2 21:19:18 2027 GMT\n  hsts: false\ndomains:\n- domain: claimglide.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/claimglide/refs/heads/main/security/claimglide-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Healthcare
- Digital Health
- Prior Authorization
- Health Insurance
- Revenue Cycle Management
- Medical Claims
- Artificial Intelligence
- Appeals
---
