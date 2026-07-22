---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: getdayjob.ai
  spf: true
hosts:
- cert_expires: Sep  7 20:52:26 2026 GMT
  host: www.getdayjob.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dayjob Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dayjob, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Dayjob
provider_slug: dayjob
slug: dayjob-domain-security
source_filename: dayjob-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getdayjob.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 20:52:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getdayjob.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dayjob/refs/heads/main/security/dayjob-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Logistics
- Transportation
- Waste Management
- Fleet Management
- Scheduling
- Route Optimization
- Artificial Intelligence
---
