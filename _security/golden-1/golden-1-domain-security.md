---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: golden1.com
  spf: true
hosts:
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: www.golden1.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Golden 1 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Golden 1 Credit Union, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Golden 1 Credit Union
provider_slug: golden-1
slug: golden-1-domain-security
source_filename: golden-1-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.golden1.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: golden1.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/golden-1/refs/heads/main/security/golden-1-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Financial-Services
- Banking
- Credit Union
- United States
- Consumer Finance
- Open Finance
- Data Aggregation
---
