---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: msc.com
  spf: true
hosts:
- cert_expires: Sep 14 23:59:59 2026 GMT
  host: www.msc.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Msc Cargo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MSC Mediterranean Shipping Company, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MSC Mediterranean Shipping Company
provider_slug: msc-cargo
slug: msc-cargo-domain-security
source_filename: msc-cargo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.msc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: msc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/msc-cargo/refs/heads/main/security/msc-cargo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Shipping
- Container Shipping
- Ocean Freight
- Logistics
- Supply Chain
- Maritime
- Cargo
- Bill of Lading
- Track and Trace
- Booking
- Instant Quote
- EDI
- EDIFACT
- IFTMIN
- DCSA
- Direct Integrations
- myMSC
- eDocs
- Geneva
---
