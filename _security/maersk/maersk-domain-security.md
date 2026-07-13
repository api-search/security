---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: maersk.com
  spf: true
hosts:
- cert_expires: Aug 28 02:20:42 2026 GMT
  host: www.maersk.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 02:24:27 2026 GMT
  host: developer.maersk.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Maersk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Maersk, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Maersk
provider_slug: maersk
slug: maersk-domain-security
source_filename: maersk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.maersk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 02:20:42 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: developer.maersk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 02:24:27 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: maersk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maersk/refs/heads/main/security/maersk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Container Shipping
- Freight
- Logistics
- Maritime
- Ports and Terminals
- Shipping
- Supply Chain
---
