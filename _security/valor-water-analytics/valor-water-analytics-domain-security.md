---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: valorwater.com
  spf: true
hosts:
- cert_expires: Jan 30 18:00:38 2027 GMT
  host: valorwater.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Valor Water Analytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Valor Water Analytics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Valor Water Analytics
provider_slug: valor-water-analytics
slug: valor-water-analytics-domain-security
source_filename: valor-water-analytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: valorwater.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 30 18:00:38 2027 GMT\n  hsts: null\ndomains:\n- domain: valorwater.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valor-water-analytics/refs/heads/main/security/valor-water-analytics-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Water
- Analytics
- Utilities
- Data
- Acquired
---
