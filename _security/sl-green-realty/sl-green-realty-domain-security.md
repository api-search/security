---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: slgreen.com
  spf: true
hosts:
- cert_expires: Sep 26 20:40:17 2026 GMT
  host: slgreen.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sl Green Realty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SL Green Realty Corp., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SL Green Realty Corp.
provider_slug: sl-green-realty
slug: sl-green-realty-domain-security
source_filename: sl-green-realty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: slgreen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 20:40:17 2026 GMT\n  hsts: false\ndomains:\n- domain: slgreen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sl-green-realty/refs/heads/main/security/sl-green-realty-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Casino Development
- Commercial Real Estate
- Manhattan
- New York City
- NYSE Listed
- Office Leasing
- Office Properties
- Property Management
- Real Estate
- REIT
---
