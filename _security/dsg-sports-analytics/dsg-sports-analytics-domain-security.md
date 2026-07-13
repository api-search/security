---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: datasportsgroup.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: dsg-api.com
  spf: false
hosts:
- cert_expires: Oct  2 21:09:48 2026 GMT
  host: datasportsgroup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 28 16:26:16 2027 GMT
  host: dsg-api.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dsg Sports Analytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DSG Sports Analytics, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DSG Sports Analytics
provider_slug: dsg-sports-analytics
slug: dsg-sports-analytics-domain-security
source_filename: dsg-sports-analytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datasportsgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 21:09:48 2026 GMT\n  hsts: false\n- host: dsg-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 28 16:26:16 2027 GMT\n  hsts: false\ndomains:\n- domain: datasportsgroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dsg-api.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dsg-sports-analytics/refs/heads/main/security/dsg-sports-analytics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Analysis
- Insights
- Sports
- Sports Data
- Live Scores
- Statistics
---
