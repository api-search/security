---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: qlik.dev
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: qlikcloud.com
  spf: true
hosts:
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: qlik.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: your-tenant.qlikcloud.com
  https: false
kind: domain-security
layout: security
method: probed
name: Qliksense Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qlik Sense APIs, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Qlik Sense APIs
provider_slug: qliksense
slug: qliksense-domain-security
source_filename: qliksense-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qlik.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: false\n- host: your-tenant.qlikcloud.com\n  https: false\ndomains:\n- domain: qlik.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n- domain: qlikcloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qliksense/refs/heads/main/security/qliksense-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Analytics
- Business Intelligence
- Cloud
- Data Visualization
- Enterprise
---
