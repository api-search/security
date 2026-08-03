---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: healthcare.com
  spf: true
hosts:
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: www.healthcare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Healthcare Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Healthcare.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Healthcare.com
provider_slug: healthcare-com
slug: healthcare-com-domain-security
source_filename: healthcare-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.healthcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: healthcare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/healthcare-com/refs/heads/main/security/healthcare-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health Insurance
- Insurance
- Healthcare
- Medicare
- Insurtech
- Marketplace
- Consumer
- Lead Generation
- Insurance Distribution
---
