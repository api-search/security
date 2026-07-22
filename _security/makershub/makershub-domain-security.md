---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: makershub.com
  spf: false
hosts:
- cert_expires: Oct  4 13:45:47 2026 GMT
  host: makershub.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Makershub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Makershub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Makershub
provider_slug: makershub
slug: makershub-domain-security
source_filename: makershub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: makershub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 13:45:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: makershub.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/makershub/refs/heads/main/security/makershub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Accounts Payable
- AP Automation
- Invoice Processing
- Accounting
- Payments
- Financial Operations
- Construction
---
