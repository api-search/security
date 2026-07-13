---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kissmetrics.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: kissmetrics.com
  spf: true
hosts:
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: www.kissmetrics.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 10:53:23 2026 GMT
  host: support.kissmetrics.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: query.kissmetrics.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Kissmetrics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kissmetrics, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kissmetrics
provider_slug: kissmetrics
slug: kissmetrics-domain-security
source_filename: kissmetrics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kissmetrics.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: false\n- host: support.kissmetrics.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 10:53:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: query.kissmetrics.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate\n    (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: kissmetrics.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: kissmetrics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kissmetrics/refs/heads/main/security/kissmetrics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Product Analytics
- Behavioral Analytics
- Marketing Analytics
- Funnels
- Cohorts
---
