---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: sendible.com
  spf: true
hosts:
- cert_expires: Sep 14 23:59:00 2026 GMT
  host: www.sendible.com
  hsts: true
  hsts_max_age: 3628800
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: developers.sendible.com
  hsts: true
  hsts_max_age: 3628800
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 16 16:40:50 2026 GMT
  host: api.sendible.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sendible Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sendible, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Sendible
provider_slug: sendible
slug: sendible-domain-security
source_filename: sendible-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sendible.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:59:00 2026 GMT\n  hsts: true\n  hsts_max_age: 3628800\n- host: developers.sendible.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 3628800\n- host: api.sendible.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 16:40:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sendible.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendible/refs/heads/main/security/sendible-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Social Media
- Social Media Management
- Agencies
- Scheduling
- Analytics
- Monitoring
---
