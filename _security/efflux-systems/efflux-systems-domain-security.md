---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: effluxsystems.com
  spf: true
hosts:
- cert_expires: Dec 29 08:29:27 2026 GMT
  host: effluxsystems.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Efflux Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Efflux Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Efflux Systems
provider_slug: efflux-systems
slug: efflux-systems-domain-security
source_filename: efflux-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: effluxsystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 08:29:27 2026 GMT\n  hsts: null\ndomains:\n- domain: effluxsystems.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/efflux-systems/refs/heads/main/security/efflux-systems-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Security
- Cybersecurity
- Attack Surface Management
- Asset Intelligence
- Asset Discovery
- Threat Intelligence
- Vulnerability Management
---
