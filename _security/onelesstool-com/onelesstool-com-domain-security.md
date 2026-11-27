---
api_specs:
- filename: onelesstool-com-decisions-api-openapi.yml
  format: yaml
  label: OneLessTool Decisions API
  slug: onelesstool-com-decisions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onelesstool-com/openapi/onelesstool-com-decisions-api-openapi.yml
- filename: onelesstool-com-discovery-api-openapi.yml
  format: yaml
  label: OneLessTool Discovery API
  slug: onelesstool-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onelesstool-com/openapi/onelesstool-com-discovery-api-openapi.yml
- filename: onelesstool-com-knowledge-api-openapi.yml
  format: yaml
  label: OneLessTool Knowledge API
  slug: onelesstool-com-knowledge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onelesstool-com/openapi/onelesstool-com-knowledge-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: onelesstool.com
  spf: true
hosts:
- cert_expires: Jan 11 11:55:04 2027 GMT
  host: onelesstool.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OneLessTool Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OneLessTool, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OneLessTool
provider_slug: onelesstool-com
slug: onelesstool-com-domain-security
source_filename: onelesstool-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onelesstool.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 11:55:04 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: onelesstool.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/onelesstool-com/security/onelesstool-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Software-as-a-Service
- Cost Optimization
- Subscription Management
- Artificial Intelligence
- Productivity
---
