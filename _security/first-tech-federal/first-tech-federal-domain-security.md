---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: firsttechfed.com
  spf: true
hosts:
- cert_expires: Sep 29 21:07:36 2026 GMT
  host: www.firsttechfed.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: First Tech Federal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for First Tech Federal Credit Union, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: First Tech Federal Credit Union
provider_slug: first-tech-federal
slug: first-tech-federal-domain-security
source_filename: first-tech-federal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.firsttechfed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 21:07:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: firsttechfed.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/first-tech-federal/refs/heads/main/security/first-tech-federal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial-Services
- Banking
- United States
- Credit Union
- Open Finance
- Data Aggregation
---
