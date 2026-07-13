---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: signl4.com
  spf: true
hosts:
- cert_expires: Sep  7 18:42:05 2026 GMT
  host: www.signl4.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 00:35:18 2026 GMT
  host: docs.signl4.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: connect.signl4.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Signl4 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SIGNL4, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SIGNL4
provider_slug: signl4
slug: signl4-domain-security
source_filename: signl4-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.signl4.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 18:42:05 2026 GMT\n  hsts: false\n- host: docs.signl4.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 00:35:18 2026 GMT\n  hsts: false\n- host: connect.signl4.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: signl4.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signl4/refs/heads/main/security/signl4-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Alerting
- Incident Management
- On-Call
- Mobile Alerts
- Notifications
- DevOps
- IT Operations
- Monitoring
---
