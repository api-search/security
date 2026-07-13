---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: transitchicago.com
  spf: true
hosts:
- cert_expires: Sep 14 17:15:30 2026 GMT
  host: www.transitchicago.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transport For Chicago Us Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transport for Chicago, US, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Transport for Chicago, US
provider_slug: transport-for-chicago-us
slug: transport-for-chicago-us-domain-security
source_filename: transport-for-chicago-us-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.transitchicago.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 17:15:30 2026 GMT\n  hsts: false\ndomains:\n- domain: transitchicago.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transport-for-chicago-us/refs/heads/main/security/transport-for-chicago-us-domain-security.yml
summary_line: TLSv1.3
tags:
- Transportation
- Public APIs
---
