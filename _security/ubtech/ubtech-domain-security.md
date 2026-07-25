---
api_specs:
- filename: ubtech-subscriptions-api-openapi.yml
  format: yaml
  label: UBTech subscriptions API
  slug: ubtech-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubtech/refs/heads/main/openapi/ubtech-subscriptions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ubtrobot.com
  spf: true
hosts:
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: ubtrobot.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- host: 127.0.0.1
  https: false
kind: domain-security
layout: security
method: probed
name: Ubtech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UBTech, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: UBTech
provider_slug: ubtech
slug: ubtech-domain-security
source_filename: ubtech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ubtrobot.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: false\n- host: 127.0.0.1\n  https: false\ndomains:\n- domain: ubtrobot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ubtech/refs/heads/main/security/ubtech-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Robotics
- Humanoid Robots
- Education Technology
- Artificial Intelligence
- Consumer Electronics
- Service Robots
---
