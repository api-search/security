---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: continuumcloud.com
  spf: true
hosts:
- cert_expires: Sep  7 16:27:07 2026 GMT
  host: continuumcloud.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Continuumcloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ContinuumCloud, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ContinuumCloud
provider_slug: continuumcloud
slug: continuumcloud-domain-security
source_filename: continuumcloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: continuumcloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 16:27:07 2026 GMT\n  hsts: false\ndomains:\n- domain: continuumcloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/continuumcloud/refs/heads/main/security/continuumcloud-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Behavioral Health
- Human Services
- Electronic Health Records
- Human Capital Management
- Patient Engagement
- Payroll
- Healthcare
- SaaS
---
