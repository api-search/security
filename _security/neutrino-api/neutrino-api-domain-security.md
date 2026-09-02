---
api_specs:
- filename: neutrino-api-data-tools-api-openapi.yml
  format: yaml
  label: Neutrino API Data Tools API
  slug: neutrino-api-data-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neutrino-api/refs/heads/main/openapi/neutrino-api-data-tools-api-openapi.yml
- filename: neutrino-api-e-commerce-api-openapi.yml
  format: yaml
  label: Neutrino API E Commerce API
  slug: neutrino-api-e-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neutrino-api/refs/heads/main/openapi/neutrino-api-e-commerce-api-openapi.yml
- filename: neutrino-api-geolocation-api-openapi.yml
  format: yaml
  label: Neutrino API Geolocation API
  slug: neutrino-api-geolocation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neutrino-api/refs/heads/main/openapi/neutrino-api-geolocation-api-openapi.yml
- filename: neutrino-api-imaging-api-openapi.yml
  format: yaml
  label: Neutrino API Imaging API
  slug: neutrino-api-imaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neutrino-api/refs/heads/main/openapi/neutrino-api-imaging-api-openapi.yml
- filename: neutrino-api-security-and-networking-api-openapi.yml
  format: yaml
  label: Neutrino API Security and Networking API
  slug: neutrino-api-security-and-networking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neutrino-api/refs/heads/main/openapi/neutrino-api-security-and-networking-api-openapi.yml
- filename: neutrino-api-telephony-api-openapi.yml
  format: yaml
  label: Neutrino API Telephony API
  slug: neutrino-api-telephony-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neutrino-api/refs/heads/main/openapi/neutrino-api-telephony-api-openapi.yml
- filename: neutrino-api-www-api-openapi.yml
  format: yaml
  label: Neutrino API WWW API
  slug: neutrino-api-www-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neutrino-api/refs/heads/main/openapi/neutrino-api-www-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: neutrinoapi.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: neutrinoapi.net
  spf: true
hosts:
- cert_expires: Feb 13 02:28:02 2027 GMT
  host: www.neutrinoapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 19:49:37 2026 GMT
  host: neutrinoapi.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 19:49:37 2026 GMT
  host: aws.neutrinoapi.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neutrino Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neutrino API, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Neutrino API
provider_slug: neutrino-api
slug: neutrino-api-domain-security
source_filename: neutrino-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.neutrinoapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 02:28:02 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: neutrinoapi.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 19:49:37 2026 GMT\n  hsts: false\n- host: aws.neutrinoapi.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 19:49:37 2026 GMT\n  hsts: false\ndomains:\n- domain: neutrinoapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: neutrinoapi.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neutrino-api/refs/heads/main/security/neutrino-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Validation
- Data Tools
- Telephony
- Communications
- SMS
- Voice
- Geolocation
- IP Intelligence
- Security
- Networking
- Anti-Fraud
- E-Commerce
- Payments
- Imaging
- Rendering
- Currency
- FX
---
