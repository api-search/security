---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nobl9.com
  spf: true
hosts:
- cert_expires: Sep 19 21:48:52 2026 GMT
  host: www.nobl9.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: docs.nobl9.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: app.nobl9.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nobl9 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nobl9, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Nobl9
provider_slug: nobl9
slug: nobl9-domain-security
source_filename: nobl9-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nobl9.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 21:48:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.nobl9.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.nobl9.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nobl9.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nobl9/refs/heads/main/security/nobl9-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Reliability
- SLO
- Service Level Objectives
- SRE
- Observability
- Error Budgets
---
