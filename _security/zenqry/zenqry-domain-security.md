---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: zenqry.com
  spf: false
hosts:
- cert_expires: Nov 26 12:07:51 2026 GMT
  host: www.zenqry.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zenqry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Björn Wilmsmann IT Services, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Björn Wilmsmann IT Services
provider_slug: zenqry
slug: zenqry-domain-security
source_filename: zenqry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zenqry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 12:07:51 2026 GMT\n  hsts: false\ndomains:\n- domain: zenqry.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/zenqry/security/zenqry-domain-security.yml
summary_line: TLSv1.3
tags:
- Backend
- BaaS
- Enterprise
- Data Integration
- REST API
---
