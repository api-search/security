---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: solsten.io
  spf: true
hosts:
- cert_expires: Oct 22 08:38:06 2026 GMT
  host: solsten.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 01:22:49 2026 GMT
  host: docs.api.solsten.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 17:13:04 2026 GMT
  host: api.solsten.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: 12Traits Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Solsten, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Solsten
provider_slug: 12traits
slug: 12traits-domain-security
source_filename: 12traits-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: solsten.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 08:38:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.api.solsten.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 01:22:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.solsten.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 17:13:04 2026 GMT\n  hsts: false\ndomains:\n- domain: solsten.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/12traits/refs/heads/main/security/12traits-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Audience Intelligence
- Psychographics
- Consumer Insights
- Analytics
- Artificial Intelligence
- Gaming
- Market Research
- Personalization
- Behavioral Data
---
