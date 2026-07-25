---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dcu.org
  spf: true
hosts:
- cert_expires: Oct 24 18:18:56 2026 GMT
  host: www.dcu.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Digital Federal Credit Union Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DCU (Digital Federal Credit Union), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DCU (Digital Federal Credit Union)
provider_slug: digital-federal-credit-union
slug: digital-federal-credit-union-domain-security
source_filename: digital-federal-credit-union-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dcu.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 18:18:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dcu.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digital-federal-credit-union/refs/heads/main/security/digital-federal-credit-union-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Services
- Banking
- United States
- Credit Union
- Consumer Banking
- Open Finance
- Data Aggregation
---
