---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: azurengine.com
  spf: true
hosts:
- cert_expires: Nov 27 09:11:48 2026 GMT
  host: azurengine.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Azurengine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azurengine, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Azurengine
provider_slug: azurengine
slug: azurengine-domain-security
source_filename: azurengine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: azurengine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 09:11:48 2026 GMT\n  hsts: null\ndomains:\n- domain: azurengine.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azurengine/refs/heads/main/security/azurengine-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Semiconductor
- Parallel Computing
- AI Hardware
- Reconfigurable Architecture
---
