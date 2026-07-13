---
api_specs:
- filename: ubiquiti-unifi-site-manager-api-openapi.yml
  format: yaml
  label: UniFi Site Manager API
  slug: unifi-site-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubiquiti/refs/heads/main/openapi/ubiquiti-unifi-site-manager-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ui.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: amplifi.com
  spf: true
hosts:
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: www.ui.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 28 23:59:59 2027 GMT
  host: developer.ui.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: amplifi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ubiquiti Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ubiquiti, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ubiquiti
provider_slug: ubiquiti
slug: ubiquiti-domain-security
source_filename: ubiquiti-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ui.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.ui.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 28 23:59:59 2027 GMT\n  hsts: false\n- host: amplifi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: ui.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: amplifi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ubiquiti/refs/heads/main/security/ubiquiti-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Networking
- WiFi
- Switching
- Routing
- Surveillance
- Access Control
- ISP
- WISP
- UniFi
- UISP
- AmpliFi
---
