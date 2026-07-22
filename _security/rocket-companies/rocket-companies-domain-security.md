---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rocketcompanies.com
  spf: false
hosts:
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: www.rocketcompanies.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rocket Companies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rocket Companies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Rocket Companies
provider_slug: rocket-companies
slug: rocket-companies-domain-security
source_filename: rocket-companies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rocketcompanies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: rocketcompanies.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rocket-companies/refs/heads/main/security/rocket-companies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Financial Services
- Mortgage
- Real Estate
- Personal Finance
- Lending
---
