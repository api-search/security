---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: maryland.gov
  spf: true
hosts:
- cert_expires: Dec 30 11:58:57 2026 GMT
  host: dat.maryland.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Maryland Department Of Assessments And Taxation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Maryland Department of Assessments and Taxation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Maryland Department of Assessments and Taxation
provider_slug: maryland-department-of-assessments-and-taxation
slug: maryland-department-of-assessments-and-taxation-domain-security
source_filename: maryland-department-of-assessments-and-taxation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dat.maryland.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 11:58:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: maryland.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/maryland-department-of-assessments-and-taxation/security/maryland-department-of-assessments-and-taxation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Government
- Real Estate
- Business Services
- Data
- Maryland
---
