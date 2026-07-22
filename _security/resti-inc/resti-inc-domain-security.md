---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: resti.cloud
  spf: true
hosts:
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: resti.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Resti Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Resti Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Resti Inc.
provider_slug: resti-inc
slug: resti-inc-domain-security
source_filename: resti-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: resti.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: resti.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resti-inc/refs/heads/main/security/resti-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Restaurant Management
- Hospitality
- HR
- Payroll
- SaaS
- Point of Sale
- Reputation Management
- Kazakhstan
---
