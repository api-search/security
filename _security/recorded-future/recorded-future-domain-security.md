---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: recordedfuture.com
  spf: true
hosts:
- cert_expires: Oct  3 02:22:31 2026 GMT
  host: www.recordedfuture.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 20 23:59:59 2027 GMT
  host: app.recordedfuture.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 23:41:39 2026 GMT
  host: support.recordedfuture.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Recorded Future Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Recorded Future, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Recorded Future
provider_slug: recorded-future
slug: recorded-future-domain-security
source_filename: recorded-future-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.recordedfuture.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 02:22:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: app.recordedfuture.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.recordedfuture.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 23:41:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: recordedfuture.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recorded-future/refs/heads/main/security/recorded-future-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cybersecurity
- Threat Intelligence
- Intelligence Cloud
- Brand Intelligence
- Identity Intelligence
- Vulnerability Intelligence
- AI Analyst
---
