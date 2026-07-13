---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:domain@zumper.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: padmapper.com
  spf: true
hosts:
- cert_expires: Mar 31 22:50:16 2027 GMT
  host: www.padmapper.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Padmapper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PadMapper, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PadMapper
provider_slug: padmapper
slug: padmapper-domain-security
source_filename: padmapper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.padmapper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 31 22:50:16 2027 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: padmapper.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:domain@zumper.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/padmapper/refs/heads/main/security/padmapper-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Rental Listings
- Apartment Search
- Map-Based Search
- Housing
- Property Discovery
- Rental Market Data
---
