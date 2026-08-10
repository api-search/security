---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: atombeamtech.com
  spf: true
hosts:
- cert_expires: Sep 27 11:36:10 2026 GMT
  host: www.atombeamtech.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: acp.atombeamtech.com
  hsts: false
  https: true
  note: AtomBeam Customer Portal SPA (CloudFront); root returns 200
  tls_version: TLSv1.3
- host: acg-api.atombeamtech.com
  hsts: false
  https: true
  note: portal backend (AWS API Gateway); every path returns 403 Forbidden
  tls_version: TLSv1.3
- host: customersupport.atombeamtech.com
  hsts: false
  https: true
  note: CNAME to Atlassian Jira Service Management; root 302s to a servicedesk login
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atombeam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AtomBeam, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: AtomBeam
provider_slug: atombeam
slug: atombeam-domain-security
source_filename: atombeam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.atombeamtech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 11:36:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: acp.atombeamtech.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: false\n  note: AtomBeam Customer Portal SPA (CloudFront); root returns 200\n- host: acg-api.atombeamtech.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: false\n  note: portal backend (AWS API Gateway); every path returns 403 Forbidden\n- host: customersupport.atombeamtech.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: false\n  note: CNAME to Atlassian Jira Service Management; root 302s to a servicedesk login\ndomains:\n- domain: atombeamtech.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atombeam/refs/heads/main/security/atombeam-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Data Compression
- Internet of Things
- Edge Computing
- Satellite Communications
- Machine Learning
- Data Management
- Defense
- Telemetry
---
