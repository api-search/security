---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: solactron.com
  spf: true
hosts:
- cert_expires: Sep 15 20:12:17 2026 GMT
  host: solactron.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Solactron Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Solactron, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Solactron
provider_slug: solactron
slug: solactron-domain-security
source_filename: solactron-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: solactron.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 20:12:17 2026 GMT\n  hsts: false\ndomains:\n- domain: solactron.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solactron/refs/heads/main/security/solactron-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Solar
- Renewable Energy
- Thin Film
- Photovoltaics
- Clean Technology
- Hardware
- Manufacturing
- Energy
---
