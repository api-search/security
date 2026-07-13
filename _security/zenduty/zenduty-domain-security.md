---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zenduty.com
  spf: true
hosts:
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: www.zenduty.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 16:03:42 2026 GMT
  host: apidocs.zenduty.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: zenduty.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zenduty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zenduty, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Zenduty
provider_slug: zenduty
slug: zenduty-domain-security
source_filename: zenduty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zenduty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.zenduty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 16:03:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: zenduty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zenduty.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenduty/refs/heads/main/security/zenduty-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Incident Management
- On-Call
- Alerting
- SRE
- DevOps
- Observability
---
