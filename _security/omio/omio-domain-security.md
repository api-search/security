---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: omio.co.uk
  spf: true
hosts:
- cert_expires: Oct 16 06:09:42 2026 GMT
  host: www.omio.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Omio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for omio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: omio
provider_slug: omio
slug: omio-domain-security
source_filename: omio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.omio.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 06:09:42 2026 GMT\n  hsts: null\ndomains:\n- domain: omio.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omio/refs/heads/main/security/omio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Travel
- Transportation
- Booking
- Mobility
- Trains
- Aggregator
- Marketplace
---
