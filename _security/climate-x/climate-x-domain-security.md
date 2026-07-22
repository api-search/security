---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: climate-x.com
  spf: true
hosts:
- cert_expires: Oct  7 16:30:49 2026 GMT
  host: www.climate-x.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Climate X Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Climate-X, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Climate-X
provider_slug: climate-x
slug: climate-x-domain-security
source_filename: climate-x-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.climate-x.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 16:30:49 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: climate-x.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/climate-x/refs/heads/main/security/climate-x-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Enterprise
- Climate Risk
- Climate Data
- Financial Risk
- Analytics
- Sustainability
- ESG
- Real Estate
- Insurance
- Banking
---
