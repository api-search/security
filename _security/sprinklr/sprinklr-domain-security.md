---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sprinklr.com
  spf: true
hosts:
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: www.sprinklr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 07:43:41 2026 GMT
  host: dev.sprinklr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 09:55:41 2026 GMT
  host: api3.sprinklr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sprinklr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sprinklr, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sprinklr
provider_slug: sprinklr
slug: sprinklr-domain-security
source_filename: sprinklr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sprinklr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: false\n- host: dev.sprinklr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 07:43:41 2026 GMT\n  hsts: null\n- host: api3.sprinklr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 09:55:41 2026 GMT\n  hsts: null\ndomains:\n- domain: sprinklr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sprinklr/refs/heads/main/security/sprinklr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Social Media Management
- Customer Experience
- Customer Service
- Marketing
- Advertising
- Listening
- Publishing
- Reporting
- Unified CXM
---
