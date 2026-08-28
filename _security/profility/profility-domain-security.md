---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: profility.com
  spf: true
hosts:
- cert_expires: Nov  3 22:40:47 2026 GMT
  host: profility.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Profility Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Profility, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Profility
provider_slug: profility
slug: profility-domain-security
source_filename: profility-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: profility.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 22:40:47 2026 GMT\n  hsts: false\ndomains:\n- domain: profility.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/profility/refs/heads/main/security/profility-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Healthcare
- Health IT
- Post-Acute Care
- Artificial Intelligence
- Predictive Analytics
- Care Coordination
- Prior Authorization
- Revenue Cycle Management
---
