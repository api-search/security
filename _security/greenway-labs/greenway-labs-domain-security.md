---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: greenwaylabs.com
  spf: false
hosts:
- cert_expires: Oct  5 16:03:57 2026 GMT
  host: greenwaylabs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Greenway Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GreenWay Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: GreenWay Labs
provider_slug: greenway-labs
slug: greenway-labs-domain-security
source_filename: greenway-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: greenwaylabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 16:03:57 2026 GMT\n  hsts: null\ndomains:\n- domain: greenwaylabs.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greenway-labs/refs/heads/main/security/greenway-labs-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
