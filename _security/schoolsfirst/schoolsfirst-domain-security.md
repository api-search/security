---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: schoolsfirstfcu.org
  spf: true
hosts:
- cert_expires: Oct 17 05:51:22 2026 GMT
  host: www.schoolsfirstfcu.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Schoolsfirst Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SchoolsFirst FCU, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: SchoolsFirst FCU
provider_slug: schoolsfirst
slug: schoolsfirst-domain-security
source_filename: schoolsfirst-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.schoolsfirstfcu.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 05:51:22 2026 GMT\n  hsts: null\ndomains:\n- domain: schoolsfirstfcu.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/schoolsfirst/refs/heads/main/security/schoolsfirst-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Financial-Services
- Banking
- United States
- Credit Union
- Open Finance
- Data Aggregation
---
