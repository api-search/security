---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pingdom.com
  spf: true
hosts:
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: www.pingdom.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: docs.pingdom.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 03:35:24 2026 GMT
  host: api.pingdom.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pingdom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pingdom, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pingdom
provider_slug: pingdom
slug: pingdom-domain-security
source_filename: pingdom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pingdom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.pingdom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: false\n- host: api.pingdom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 03:35:24 2026 GMT\n  hsts: null\ndomains:\n- domain: pingdom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pingdom/refs/heads/main/security/pingdom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Monitoring
- Uptime Monitoring
- Website Monitoring
- Performance Monitoring
- Real User Monitoring
- Synthetic Monitoring
- Observability
---
