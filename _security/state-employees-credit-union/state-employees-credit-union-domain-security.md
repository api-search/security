---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ncsecu.org
  spf: true
hosts:
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: www.ncsecu.org
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: State Employees Credit Union Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for State Employees'' Credit Union, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: State Employees' Credit Union
provider_slug: state-employees-credit-union
slug: state-employees-credit-union-domain-security
source_filename: state-employees-credit-union-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ncsecu.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: ncsecu.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/state-employees-credit-union/refs/heads/main/security/state-employees-credit-union-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Services
- Banking
- Credit Union
- United States
- North Carolina
- Open Finance
- Data Aggregation
---
