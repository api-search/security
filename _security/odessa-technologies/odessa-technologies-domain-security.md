---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: odessainc.com
  spf: true
hosts:
- cert_expires: Oct  2 12:25:56 2026 GMT
  host: www.odessainc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Odessa Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Odessa Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Odessa Technologies
provider_slug: odessa-technologies
slug: odessa-technologies-domain-security
source_filename: odessa-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.odessainc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:25:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: odessainc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/odessa-technologies/refs/heads/main/security/odessa-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Asset Finance
- Lease Management
- Loan Management
- Equipment Finance
- Auto Finance
- Originations
- Servicing
- Remarketing
- Low Code
- Financial Services
---
