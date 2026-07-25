---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: finaeo.com
  spf: false
hosts:
- cert_expires: Sep 29 21:32:52 2026 GMT
  host: www.finaeo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Finaeo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Finaeo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Finaeo
provider_slug: finaeo
slug: finaeo-domain-security
source_filename: finaeo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.finaeo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 21:32:52 2026 GMT\n  hsts: null\ndomains:\n- domain: finaeo.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finaeo/refs/heads/main/security/finaeo-domain-security.yml
summary_line: TLSv1.3
tags:
- Insurance
- Canada
- Life Insurance
- Insurtech
- Broker
- Agency Management
- Marketplace
- Distribution
- Quoting
- Policy Administration
---
