---
api_specs:
- filename: thespacedevs-ll2-api-openapi.yml
  format: yaml
  label: TheSpaceDevs Launch Library 2 API
  slug: thespacedevs-ll2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thespacedevs-ll2-api/refs/heads/main/openapi/thespacedevs-ll2-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: thespacedevs.com
  spf: true
hosts:
- cert_expires: Aug 29 05:16:03 2026 GMT
  host: thespacedevs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 05:16:03 2026 GMT
  host: ll.thespacedevs.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thespacedevs Ll2 Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TheSpaceDevs LL2 API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: TheSpaceDevs LL2 API
provider_slug: thespacedevs-ll2-api
slug: thespacedevs-ll2-api-domain-security
source_filename: thespacedevs-ll2-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thespacedevs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 05:16:03 2026 GMT\n  hsts: false\n- host: ll.thespacedevs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 05:16:03 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: thespacedevs.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thespacedevs-ll2-api/refs/heads/main/security/thespacedevs-ll2-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Space
- Satellites
- Launches
- Rockets
- Astronauts
---
