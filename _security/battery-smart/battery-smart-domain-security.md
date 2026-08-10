---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: batterysmart.in
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: upgrid.in
  note: Battery Smart's engineering domain (Upgrid Solutions Private Limited). No DMARC record published at _dmarc.upgrid.in and no CAA record on the zone.
  spf: true
  spf_record: v=spf1 include:_spf.google.com ~all
hosts:
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: www.batterysmart.in
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: api.upgrid.in
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Production API host behind the Battery Smart Driver and Partner mobile apps; root returns {"message":"Battery Smart API"}. Discovered via Certificate Transparency, not from any published apis.yml/OpenAPI pointer — Battery Smart publishes no API documentation for it. Probed anonymously; no operations enumerated.
  security_headers:
    access_control_allow_origin: '*'
    content_security_policy: default-src 'none';base-uri 'none';form-action 'none';frame-ancestors 'none'
    cross_origin_opener_policy: same-origin
    referrer_policy: no-referrer
    x_content_type_options: nosniff
    x_frame_options: DENY
  server: Express (X-Powered-By header exposed)
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Battery Smart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Battery Smart, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Battery Smart
provider_slug: battery-smart
slug: battery-smart-domain-security
source_filename: battery-smart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.batterysmart.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: false\n- host: api.upgrid.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: >-\n    Production API host behind the Battery Smart Driver and Partner mobile apps;\n    root returns {\"message\":\"Battery Smart API\"}. Discovered via Certificate\n    Transparency, not from any published apis.yml/OpenAPI pointer — Battery Smart\n    publishes no API documentation for it. Probed anonymously; no operations\n    enumerated.\n  security_headers:\n    content_security_policy: \"default-src 'none';base-uri 'none';form-action 'none';frame-ancestors 'none'\"\n    x_content_type_options: nosniff\n    x_frame_options: DENY\n    referrer_policy: no-referrer\n\
  \    cross_origin_opener_policy: same-origin\n    access_control_allow_origin: '*'\n  server: Express (X-Powered-By header exposed)\ndomains:\n- domain: batterysmart.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: upgrid.in\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com ~all\n  dmarc: false\n  note: >-\n    Battery Smart's engineering domain (Upgrid Solutions Private Limited). No DMARC\n    record published at _dmarc.upgrid.in and no CAA record on the zone.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/battery-smart/refs/heads/main/security/battery-smart-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Battery Swapping
- Electric Vehicles
- EV Infrastructure
- Battery as a Service
- Energy
- Clean Energy
- Mobility
- Two Wheelers
- Three Wheelers
- Last Mile Delivery
- India
---
