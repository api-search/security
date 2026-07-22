---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: viajanet.com.br
  spf: true
hosts:
- cert_expires: Sep 20 02:28:13 2026 GMT
  host: www.viajanet.com.br
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Viajanet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Viajanet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Viajanet
provider_slug: viajanet
slug: viajanet-domain-security
source_filename: viajanet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.viajanet.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 02:28:13 2026 GMT\n  hsts: false\ndomains:\n- domain: viajanet.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/viajanet/refs/heads/main/security/viajanet-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Travel
- Online Travel Agency
- Flights
- Hotels
- Booking
- Brazil
- E-commerce
---
