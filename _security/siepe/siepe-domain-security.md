---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: siepe.com
  spf: true
hosts:
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: www.siepe.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Siepe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Siepe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Siepe
provider_slug: siepe
slug: siepe-domain-security
source_filename: siepe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.siepe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: siepe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/siepe/refs/heads/main/security/siepe-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Financial-Services
- Private Credit
- CLO
- Alternative Investments
- Portfolio-Management
- Data Management
- Fund Administration
- Middle Office
- Managed Service
- Fintech
---
