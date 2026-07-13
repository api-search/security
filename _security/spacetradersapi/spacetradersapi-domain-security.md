---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: spacetraders.io
  spf: true
hosts:
- cert_expires: Aug 23 09:59:35 2026 GMT
  host: spacetraders.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spacetradersapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SpaceTradersAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: SpaceTradersAPI
provider_slug: spacetradersapi
slug: spacetradersapi-domain-security
source_filename: spacetradersapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spacetraders.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 09:59:35 2026 GMT\n  hsts: false\ndomains:\n- domain: spacetraders.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spacetradersapi/refs/heads/main/security/spacetradersapi-domain-security.yml
summary_line: TLSv1.3
tags:
- Games And Comics
- Public APIs
---
