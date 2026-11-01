---
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getconvey.com
  spf: true
hosts:
- cert_expires: Mar 28 23:59:59 2027 GMT
  host: getconvey.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Getconvey Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Convey, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Convey
provider_slug: getconvey-com
slug: getconvey-com-domain-security
source_filename: getconvey-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getconvey.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 28 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: getconvey.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/getconvey-com/security/getconvey-com-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Supply Chain
- Decision Intelligence
- Transportation Management
- Visibility
- AI Orchestration
- Yard Management
- eCommerce Logistics
---
