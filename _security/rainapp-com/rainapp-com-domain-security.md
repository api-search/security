---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rainapp.com
  spf: true
hosts:
- cert_expires: Jan 10 18:16:39 2027 GMT
  host: rainapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rainapp Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rain, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rain
provider_slug: rainapp-com
slug: rainapp-com-domain-security
source_filename: rainapp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rainapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 18:16:39 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rainapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/rainapp-com/security/rainapp-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- FinancialHealth
- EmployeeBenefits
- FinTech
- AI
---
