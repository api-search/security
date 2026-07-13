---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: trafiklab.se
  spf: true
hosts:
- cert_expires: Sep 24 06:14:30 2026 GMT
  host: www.trafiklab.se
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transport For Sweden Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transport for Sweden, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Transport for Sweden
provider_slug: transport-for-sweden
slug: transport-for-sweden-domain-security
source_filename: transport-for-sweden-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trafiklab.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 06:14:30 2026 GMT\n  hsts: false\ndomains:\n- domain: trafiklab.se\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transport-for-sweden/refs/heads/main/security/transport-for-sweden-domain-security.yml
summary_line: TLSv1.3
tags:
- Transportation
- Public APIs
---
