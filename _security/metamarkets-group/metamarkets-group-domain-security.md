---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: metamarkets.com
  spf: true
hosts:
- cert_expires: Oct  2 11:27:22 2026 GMT
  host: docs.metamarkets.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: rt-evaluate.metamarkets.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Metamarkets Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metamarkets Group, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Metamarkets Group
provider_slug: metamarkets-group
slug: metamarkets-group-domain-security
source_filename: metamarkets-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.metamarkets.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 11:27:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rt-evaluate.metamarkets.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate\n    (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: metamarkets.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metamarkets-group/refs/heads/main/security/metamarkets-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- AdTech
- Analytics
- Programmatic Advertising
- Real-Time Data
- Data Ingestion
- OpenRTB
- Dashboards
---
