---
api_specs:
- filename: midax402-com-badge-api-openapi.yml
  format: yaml
  label: MIDAX402 Badge API
  slug: midax402-com-badge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/midax402-com/openapi/midax402-com-badge-api-openapi.yml
- filename: midax402-com-midas-ops-api-openapi.yml
  format: yaml
  label: MIDAX402 Midas Ops API
  slug: midax402-com-midas-ops-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/midax402-com/openapi/midax402-com-midas-ops-api-openapi.yml
description: ''
domains:
- caa:
  - midax402.onrender.com.
  - gcp-us-west1-1.origin.onrender.com.
  - gcp-us-west1-1.origin.onrender.com.cdn.cloudflare.net.
  dmarc: false
  dnssec: true
  domain: midax402.com
  spf: true
hosts:
- cert_expires: Feb  1 06:22:01 2027 GMT
  host: midax402.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MIDAX402 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MIDAX402, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: MIDAX402
provider_slug: midax402-com
slug: midax402-com-domain-security
source_filename: midax402-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: midax402.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 06:22:01 2027 GMT\n  hsts: null\ndomains:\n- domain: midax402.com\n  dnssec: true\n  caa:\n  - midax402.onrender.com.\n  - gcp-us-west1-1.origin.onrender.com.\n  - gcp-us-west1-1.origin.onrender.com.cdn.cloudflare.net.\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/midax402-com/security/midax402-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Verification
- x402
- Data Intelligence
---
