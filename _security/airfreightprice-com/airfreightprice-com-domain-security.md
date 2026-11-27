---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: airfreightprice.com
  spf: true
hosts:
- cert_expires: Dec 24 20:46:51 2026 GMT
  host: airfreightprice.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Air Freight Price Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Air Freight Price, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Air Freight Price
provider_slug: airfreightprice-com
slug: airfreightprice-com-domain-security
source_filename: airfreightprice-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: airfreightprice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 20:46:51 2026 GMT\n  hsts: false\ndomains:\n- domain: airfreightprice.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/airfreightprice-com/security/airfreightprice-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Logistics
- Freight
- Shipping
- Rate Calculator
- Air Cargo
---
