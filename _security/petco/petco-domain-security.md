---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: petco.com
  spf: true
hosts:
- cert_expires: Oct  8 09:05:35 2026 GMT
  host: www.petco.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: developer.petco.com
  https: false
- host: api.petco.com
  https: false
kind: domain-security
layout: security
method: probed
name: Petco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Petco Animal Supplies, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Petco Animal Supplies
provider_slug: petco
slug: petco-domain-security
source_filename: petco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.petco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 09:05:35 2026 GMT\n  hsts: null\n- host: developer.petco.com\n  https: false\n- host: api.petco.com\n  https: false\ndomains:\n- domain: petco.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/petco/refs/heads/main/security/petco-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Pet Care
- Retail
- Veterinary
---
