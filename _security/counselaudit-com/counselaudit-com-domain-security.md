---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: counselaudit.com
  spf: true
hosts:
- cert_expires: Dec 24 14:13:14 2026 GMT
  host: counselaudit.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CounselAudit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CounselAudit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CounselAudit
provider_slug: counselaudit-com
slug: counselaudit-com-domain-security
source_filename: counselaudit-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: counselaudit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 14:13:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: counselaudit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/counselaudit-com/security/counselaudit-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Legal Tech
- Legal Billing
- Invoice Review
- E-Billing
- Outside Counsel Guidelines
- Artificial Intelligence
- MCP
---
