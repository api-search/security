---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gro-intelligence.com
  spf: false
hosts:
- cert_expires: Nov 30 17:34:14 2026 GMT
  host: gro-intelligence.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.gro-intelligence.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''api.gro-int'
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Gro Intelligence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gro Intelligence, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Gro Intelligence
provider_slug: gro-intelligence
slug: gro-intelligence-domain-security
source_filename: gro-intelligence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gro-intelligence.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 17:34:14 2026 GMT\n  hsts: null\n- host: api.gro-intelligence.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''api.gro-int'\n  hsts: null\ndomains:\n- domain: gro-intelligence.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gro-intelligence/refs/heads/main/security/gro-intelligence-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Agriculture
- Climate
- Data
- Analytics
- Satellite Imagery
- Commodities
- Weather
- Food Security
- Time Series
- Defunct
---
