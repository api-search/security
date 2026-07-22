---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: magnite.com
  spf: true
hosts:
- cert_expires: Aug 15 18:43:09 2026 GMT
  host: www.magnite.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rubicon Project Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rubicon Project, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rubicon Project
provider_slug: rubicon-project
slug: rubicon-project-domain-security
source_filename: rubicon-project-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.magnite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 18:43:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: magnite.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rubicon-project/refs/heads/main/security/rubicon-project-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- AdTech
- Programmatic Advertising
- Sell-Side Platform
- SSP
- Real-Time Bidding
- Connected TV
- Media
---
