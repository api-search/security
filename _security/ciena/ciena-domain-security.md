---
api_specs:
- filename: ciena-blue-planet-openapi.yml
  format: yaml
  label: Ciena Blue Planet Open API
  slug: blue-planet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ciena/refs/heads/main/openapi/ciena-blue-planet-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ciena.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blueplanet.com
  spf: true
hosts:
- cert_expires: Sep 30 21:27:38 2026 GMT
  host: www.ciena.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: developer.blueplanet.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 07:47:35 2026 GMT
  host: www.blueplanet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ciena Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ciena, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ciena
provider_slug: ciena
slug: ciena-domain-security
source_filename: ciena-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ciena.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 21:27:38 2026 GMT\n  hsts: null\n- host: developer.blueplanet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: false\n- host: www.blueplanet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 07:47:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ciena.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: blueplanet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ciena/refs/heads/main/security/ciena-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- MEF
- NETCONF
- Network Automation
- Network Management
- Optical
- RESTCONF
- SDN
- Telecom
- TM Forum
- Fortune 1000
---
