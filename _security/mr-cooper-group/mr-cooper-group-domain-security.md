---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mrcooper.com
  spf: true
hosts:
- cert_expires: Oct  5 20:30:13 2026 GMT
  host: www.mrcooper.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mr Cooper Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mr. Cooper Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Mr. Cooper Group
provider_slug: mr-cooper-group
slug: mr-cooper-group-domain-security
source_filename: mr-cooper-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mrcooper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 20:30:13 2026 GMT\n  hsts: null\ndomains:\n- domain: mrcooper.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mr-cooper-group/refs/heads/main/security/mr-cooper-group-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Mortgage
- Mortgage Servicing
- Financial Services
- Real Estate
- Consumer Finance
- Acquired
- Rocket Companies
---
