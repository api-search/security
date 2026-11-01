---
api_specs:
- filename: qikpod-com-openapi-generated.yml
  format: yaml
  label: QikPod API
  slug: qikpod-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qikpod-com/openapi/_ae-authored/qikpod-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: qikpod.com
  spf: true
hosts:
- host: www.qikpod.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Qikpod Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QikPod, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: QikPod
provider_slug: qikpod-com
slug: qikpod-com-domain-security
source_filename: qikpod-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qikpod.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: qikpod.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/qikpod-com/security/qikpod-com-domain-security.yml
summary_line: DMARC
tags:
- Logistics
- Parcel
- Automation
- Robotics
- IoT
---
