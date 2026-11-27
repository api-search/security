---
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: tariffschart.com
  spf: true
hosts:
- cert_expires: Jan 11 16:04:00 2027 GMT
  host: tariffschart.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: TariffChart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TariffChart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TariffChart
provider_slug: tariffschart-com
slug: tariffschart-com-domain-security
source_filename: tariffschart-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tariffschart.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 16:04:00 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tariffschart.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/tariffschart-com/security/tariffschart-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Tariff
- Landed Cost
- Import Duty
- HS Lookup
---
