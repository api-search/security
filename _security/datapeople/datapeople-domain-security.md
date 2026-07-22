---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: datapeople.io
  spf: true
hosts:
- cert_expires: Sep 23 02:47:50 2026 GMT
  host: datapeople.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datapeople Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DataPeople, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DataPeople
provider_slug: datapeople
slug: datapeople-domain-security
source_filename: datapeople-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datapeople.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 02:47:50 2026 GMT\n  hsts: false\ndomains:\n- domain: datapeople.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datapeople/refs/heads/main/security/datapeople-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Recruiting
- Human Resources
- Job Descriptions
- Talent Acquisition
- Hiring
- Analytics
- Artificial Intelligence
- ATS Integrations
---
