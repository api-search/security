---
api_specs:
- filename: ipqualityscore-openapi.yml
  format: yaml
  label: IP Reputation & Proxy/VPN Detection API
  slug: ip-reputation-proxy-vpn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-openapi.yml
- filename: ipqualityscore-openapi.yml
  format: yaml
  label: Email Validation API
  slug: email-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-openapi.yml
- filename: ipqualityscore-openapi.yml
  format: yaml
  label: Phone Number Validation API
  slug: phone-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-openapi.yml
- filename: ipqualityscore-openapi.yml
  format: yaml
  label: Malicious URL Scanner API
  slug: malicious-url-scanner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-openapi.yml
- filename: ipqualityscore-openapi.yml
  format: yaml
  label: Device Fingerprint API
  slug: device-fingerprint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-openapi.yml
- filename: ipqualityscore-openapi.yml
  format: yaml
  label: Transaction Scoring API
  slug: transaction-scoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-openapi.yml
- filename: ipqualityscore-openapi.yml
  format: yaml
  label: Leaked Data (Dark Web) API
  slug: leaked-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ipqualityscore.com
  spf: true
hosts:
- cert_expires: Sep 25 10:36:38 2026 GMT
  host: www.ipqualityscore.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ipqualityscore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IPQualityScore, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: IPQualityScore
provider_slug: ipqualityscore
slug: ipqualityscore-domain-security
source_filename: ipqualityscore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ipqualityscore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 10:36:38 2026 GMT\n  hsts: false\ndomains:\n- domain: ipqualityscore.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/security/ipqualityscore-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fraud Prevention
- IP Reputation
- Proxy Detection
- Email Validation
- Threat Intelligence
---
