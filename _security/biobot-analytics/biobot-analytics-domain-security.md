---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: biobot.io
  spf: true
hosts:
- cert_expires: Oct  4 21:25:19 2026 GMT
  host: biobot.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Biobot Analytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Biobot Analytics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Biobot Analytics
provider_slug: biobot-analytics
slug: biobot-analytics-domain-security
source_filename: biobot-analytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: biobot.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 21:25:19 2026 GMT\n  hsts: false\ndomains:\n- domain: biobot.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biobot-analytics/refs/heads/main/security/biobot-analytics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Wastewater
- Epidemiology
- Public Health
- Data Intelligence
- Life Sciences
- Government
- Biotech
---
