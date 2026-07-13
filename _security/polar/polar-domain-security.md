---
api_specs:
- filename: swagger.yaml
  format: yaml
  label: Polar AccessLink API
  slug: polar-accesslink-api
  spec_type: OpenAPI
  url: https://www.polar.com/accesslink-api/swagger.yaml
- filename: swagger.yaml
  format: yaml
  label: Polar TeamPro API
  slug: polar-teampro-api
  spec_type: OpenAPI
  url: https://www.polar.com/teampro-api/swagger.yaml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: polar.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: polaraccesslink.com
  spf: false
hosts:
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: www.polar.com
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: flow.polar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: www.polaraccesslink.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Polar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polar, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Polar
provider_slug: polar
slug: polar-domain-security
source_filename: polar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.polar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\n- host: flow.polar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: false\n- host: www.polaraccesslink.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: polar.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: polaraccesslink.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/security/polar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fitness
- Health
- Wearables
- Heart Rate
- Sports
- Training
- Sleep
- Activity Tracking
- Sensors
- Bluetooth
---
