---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: transport.rest
  spf: false
hosts:
- cert_expires: Sep 29 09:54:08 2026 GMT
  host: transport.rest
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transport Rest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for transport.rest, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: transport.rest
provider_slug: transport-rest
slug: transport-rest-domain-security
source_filename: transport-rest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: transport.rest\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 09:54:08 2026 GMT\n  hsts: false\ndomains:\n- domain: transport.rest\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transport-rest/refs/heads/main/security/transport-rest-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Transportation
- Public APIs
---
