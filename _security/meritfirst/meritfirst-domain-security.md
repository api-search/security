---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: meritfirst.us
  spf: true
hosts:
- cert_expires: Sep 28 19:16:06 2026 GMT
  host: meritfirst.us
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 08:56:42 2026 GMT
  host: www.meritfirst.us
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Meritfirst Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meritfirst, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Meritfirst
provider_slug: meritfirst
slug: meritfirst-domain-security
source_filename: meritfirst-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meritfirst.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 19:16:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.meritfirst.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 08:56:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: meritfirst.us\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meritfirst/refs/heads/main/security/meritfirst-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Hiring
- Recruiting
- Assessments
- Talent
- Skills-Based Hiring
- MCP
---
