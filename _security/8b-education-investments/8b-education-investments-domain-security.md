---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 8b.africa
  spf: true
hosts:
- cert_expires: Nov 12 15:42:28 2026 GMT
  host: www.8b.africa
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 8B Education Investments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 8B Education Investments, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 8B Education Investments
provider_slug: 8b-education-investments
slug: 8b-education-investments-domain-security
source_filename: 8b-education-investments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.8b.africa\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 15:42:28 2026 GMT\n  hsts: false\ndomains:\n- domain: 8b.africa\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/8b-education-investments/refs/heads/main/security/8b-education-investments-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Education
- Student Loans
- Financial Services
- Lending
- FinTech
- Africa
- Higher Education
- Study Abroad
- Community
---
