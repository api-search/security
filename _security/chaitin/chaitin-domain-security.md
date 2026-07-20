---
api_specs:
- filename: chaitin-safeline-openapi-original.json
  format: json
  label: SafeLine WAF Open API
  slug: safeline-waf-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaitin/refs/heads/main/openapi/chaitin-safeline-openapi-original.json
- filename: chaitin-cloudatlas-openapi-original.yaml
  format: yaml
  label: Cloud Atlas OpenAPI
  slug: cloud-atlas-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaitin/refs/heads/main/openapi/chaitin-cloudatlas-openapi-original.yaml
- filename: chaitin-apisec-openapi-original.json
  format: json
  label: APISec Management API
  slug: apisec-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaitin/refs/heads/main/openapi/chaitin-apisec-openapi-original.json
- filename: chaitin-veinmind-openapi-original.json
  format: json
  label: VeinMind API
  slug: veinmind-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaitin/refs/heads/main/openapi/chaitin-veinmind-openapi-original.json
- filename: chaitin-ddr-openapi-original.json
  format: json
  label: DDR API
  slug: ddr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaitin/refs/heads/main/openapi/chaitin-ddr-openapi-original.json
- filename: chaitin-dsensor-openapi-original.json
  format: json
  label: D-Sensor API
  slug: d-sensor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chaitin/refs/heads/main/openapi/chaitin-dsensor-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chaitin.cn
  spf: true
hosts:
- cert_expires: Sep 23 02:55:57 2026 GMT
  host: chaitin.cn
  hsts: true
  hsts_max_age: 5184000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Chaitin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chaitin Tech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Chaitin Tech
provider_slug: chaitin
slug: chaitin-domain-security
source_filename: chaitin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chaitin.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 23 02:55:57 2026 GMT\n  hsts: true\n  hsts_max_age: 5184000\ndomains:\n- domain: chaitin.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chaitin/refs/heads/main/security/chaitin-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Security
- Web Application Firewall
- WAF
- Cybersecurity
- API Security
- Container Security
- Vulnerability Scanning
- DevSecOps
- Company
---
