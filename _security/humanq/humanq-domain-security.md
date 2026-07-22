---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: humanq.com
  spf: true
hosts:
- cert_expires: Aug 27 05:15:03 2026 GMT
  host: humanq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Humanq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HumanQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HumanQ
provider_slug: humanq
slug: humanq-domain-security
source_filename: humanq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: humanq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 05:15:03 2026 GMT\n  hsts: false\ndomains:\n- domain: humanq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humanq/refs/heads/main/security/humanq-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Execution
- Facilitation
- Team Productivity
- Leadership Development
- Enterprise Software
- Coaching
---
