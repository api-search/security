---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sunrise-sunset.org
  spf: true
hosts:
- cert_expires: Aug 19 02:46:15 2026 GMT
  host: sunrise-sunset.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sunrise And Sunset Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sunrise and Sunset, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Sunrise and Sunset
provider_slug: sunrise-and-sunset
slug: sunrise-and-sunset-domain-security
source_filename: sunrise-and-sunset-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sunrise-sunset.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 02:46:15 2026 GMT\n  hsts: false\ndomains:\n- domain: sunrise-sunset.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sunrise-and-sunset/refs/heads/main/security/sunrise-and-sunset-domain-security.yml
summary_line: TLSv1.3
tags:
- Science And Math
- Public APIs
---
