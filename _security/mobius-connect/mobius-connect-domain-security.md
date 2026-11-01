---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mobius-connect.com
  spf: true
hosts:
- cert_expires: Nov 25 07:18:35 2026 GMT
  host: mobius-connect.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mobius Connect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gozynta, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Gozynta
provider_slug: mobius-connect
slug: mobius-connect-domain-security
source_filename: mobius-connect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mobius-connect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 07:18:35 2026 GMT\n  hsts: false\ndomains:\n- domain: mobius-connect.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mobius-connect/security/mobius-connect-domain-security.yml
summary_line: TLSv1.3
tags:
- IoT
- Connectivity
- Integration
- Data Processing
- Platform
---
