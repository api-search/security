---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: translink.ca
  spf: true
hosts:
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: developer.translink.ca
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transport For Vancouver Canada Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transport for Vancouver, Canada, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Transport for Vancouver, Canada
provider_slug: transport-for-vancouver-canada
slug: transport-for-vancouver-canada-domain-security
source_filename: transport-for-vancouver-canada-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.translink.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: translink.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transport-for-vancouver-canada/refs/heads/main/security/transport-for-vancouver-canada-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Transportation
- Public APIs
---
