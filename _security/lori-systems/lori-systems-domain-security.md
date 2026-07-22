---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lorisystems.com
  spf: true
hosts:
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: lorisystems.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lori Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lori Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lori Systems
provider_slug: lori-systems
slug: lori-systems-domain-security
source_filename: lori-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lorisystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: lorisystems.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lori-systems/refs/heads/main/security/lori-systems-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Logistics
- Freight
- Trucking
- Cargo
- Supply Chain
- Transportation
- Marketplace
- Africa
- East Africa
- West Africa
- Kenya
- Nigeria
- Uganda
- Digital Freight
- Last Mile
---
