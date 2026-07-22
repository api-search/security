---
api_specs:
- filename: replicated-vendor-api-v3-openapi-original.json
  format: json
  label: Replicated Vendor API v3
  slug: replicated-vendor-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicated/refs/heads/main/openapi/replicated-vendor-api-v3-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@replicated.com"
  - 0 issue "amazon.com"
  - 0 issue "cloudflare.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: replicated.com
  spf: true
hosts:
- cert_expires: Oct 16 08:39:53 2026 GMT
  host: replicated.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 03:43:31 2026 GMT
  host: api.replicated.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Replicated Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Replicated, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Replicated
provider_slug: replicated
slug: replicated-domain-security
source_filename: replicated-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: replicated.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 08:39:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.replicated.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:43:31 2026 GMT\n  hsts: null\ndomains:\n- domain: replicated.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@replicated.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"cloudflare.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/replicated/refs/heads/main/security/replicated-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Developer Tools
- Software Distribution
- Kubernetes
- On-Premises
- Application Delivery
- Air Gap
- Licensing
---
