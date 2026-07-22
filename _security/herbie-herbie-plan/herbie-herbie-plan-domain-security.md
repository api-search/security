---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: herbieplan.com
  spf: true
hosts:
- cert_expires: Sep  5 15:08:02 2026 GMT
  host: herbieplan.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Herbie Herbie Plan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Herbie, Herbie Plan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Herbie, Herbie Plan
provider_slug: herbie-herbie-plan
slug: herbie-herbie-plan-domain-security
source_filename: herbie-herbie-plan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: herbieplan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 15:08:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: herbieplan.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/herbie-herbie-plan/refs/heads/main/security/herbie-herbie-plan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Estate Planning
- Legal Technology
- Wills and Trusts
- Artificial Intelligence
- Wealth Management
- Document Automation
---
