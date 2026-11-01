---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: globalexchangerates.org
  spf: true
hosts:
- cert_expires: Jan 22 18:02:18 2027 GMT
  host: globalexchangerates.org
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Globalexchangerates Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for globalexchangerates-org, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: globalexchangerates-org
provider_slug: globalexchangerates-org
slug: globalexchangerates-org-domain-security
source_filename: globalexchangerates-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: globalexchangerates.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 18:02:18 2027 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: globalexchangerates.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/globalexchangerates-org/security/globalexchangerates-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Finance
- API
- ExchangeRates
- ERP
---
