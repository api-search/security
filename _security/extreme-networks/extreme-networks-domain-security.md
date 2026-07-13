---
api_specs:
- filename: extremecloud-iq-openapi.yml
  format: yaml
  label: ExtremeCloud IQ API
  slug: extremecloud-iq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/extreme-networks/refs/heads/main/openapi/extremecloud-iq-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: extremenetworks.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: extremecloudiq.com
  spf: true
hosts:
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: www.extremenetworks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: developer.extremecloudiq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: api.extremecloudiq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Extreme Networks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Extreme Networks, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Extreme Networks
provider_slug: extreme-networks
slug: extreme-networks-domain-security
source_filename: extreme-networks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.extremenetworks.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.extremecloudiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: false\n- host: api.extremecloudiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: extremenetworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: extremecloudiq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/extreme-networks/refs/heads/main/security/extreme-networks-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Networking
- Wireless
- Wired
- Switching
- Wi-Fi
- Wi-Fi 7
- Cloud Management
- SD-WAN
- Network Security
- Network Management
- AI Networking
- Enterprise
---
