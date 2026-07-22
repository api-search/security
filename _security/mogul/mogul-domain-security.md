---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: onmogul.com
  spf: true
hosts:
- cert_expires: Aug 31 08:44:58 2026 GMT
  host: onmogul.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mogul Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mogul, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Mogul
provider_slug: mogul
slug: mogul-domain-security
source_filename: mogul-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onmogul.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 08:44:58 2026 GMT\n  hsts: false\ndomains:\n- domain: onmogul.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mogul/refs/heads/main/security/mogul-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Executive Search
- Executive Training
- Leadership Development
- Advisory
- AI Transformation
- Human Resources
- Consulting
---
