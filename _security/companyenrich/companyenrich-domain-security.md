---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: companyenrich.com
  spf: true
hosts:
- cert_expires: Nov 29 16:30:21 2026 GMT
  host: companyenrich.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Companyenrich Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CompanyEnrich, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CompanyEnrich
provider_slug: companyenrich
slug: companyenrich-domain-security
source_filename: companyenrich-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: companyenrich.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 16:30:21 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: companyenrich.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/companyenrich/refs/heads/main/security/companyenrich-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- B2B
- Data
- Data Enrichment
- Artificial Intelligence
---
