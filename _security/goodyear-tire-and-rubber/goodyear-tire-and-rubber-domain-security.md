---
api_specs:
- filename: sightline-api.yml
  format: yaml
  label: Goodyear SightLine API
  slug: sightline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodyear-tire-and-rubber/refs/heads/main/openapi/sightline-api.yml
- filename: gaas-portal.yml
  format: yaml
  label: Goodyear API Management Portal
  slug: gaas-portal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goodyear-tire-and-rubber/refs/heads/main/openapi/gaas-portal.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: goodyear.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: goodyearsightline.com
  spf: true
hosts:
- cert_expires: Sep 11 05:08:36 2026 GMT
  host: www.goodyear.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: developer.goodyearsightline.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: gaas-portal.goodyear.com
  https: false
kind: domain-security
layout: security
method: probed
name: Goodyear Tire And Rubber Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Goodyear Tire & Rubber, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Goodyear Tire & Rubber
provider_slug: goodyear-tire-and-rubber
slug: goodyear-tire-and-rubber-domain-security
source_filename: goodyear-tire-and-rubber-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.goodyear.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 05:08:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.goodyearsightline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gaas-portal.goodyear.com\n  https: false\ndomains:\n- domain: goodyear.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: goodyearsightline.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goodyear-tire-and-rubber/refs/heads/main/security/goodyear-tire-and-rubber-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Connected Vehicles
- Fleet Management
- IoT
- Telematics
- Tires
---
