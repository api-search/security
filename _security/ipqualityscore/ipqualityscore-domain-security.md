---
api_specs:
- filename: ipqualityscore-device-fingerprint-api-openapi.yml
  format: yaml
  label: IPQualityScore Device Fingerprint API
  slug: ipqualityscore-device-fingerprint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-device-fingerprint-api-openapi.yml
- filename: ipqualityscore-email-validation-api-openapi.yml
  format: yaml
  label: IPQualityScore Email Validation API
  slug: ipqualityscore-email-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-email-validation-api-openapi.yml
- filename: ipqualityscore-ip-reputation-api-openapi.yml
  format: yaml
  label: IPQualityScore IP Reputation API
  slug: ipqualityscore-ip-reputation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-ip-reputation-api-openapi.yml
- filename: ipqualityscore-leaked-data-api-openapi.yml
  format: yaml
  label: IPQualityScore Leaked Data API
  slug: ipqualityscore-leaked-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-leaked-data-api-openapi.yml
- filename: ipqualityscore-phone-validation-api-openapi.yml
  format: yaml
  label: IPQualityScore Phone Validation API
  slug: ipqualityscore-phone-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-phone-validation-api-openapi.yml
- filename: ipqualityscore-url-scanner-api-openapi.yml
  format: yaml
  label: IPQualityScore URL Scanner API
  slug: ipqualityscore-url-scanner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipqualityscore/refs/heads/main/openapi/ipqualityscore-url-scanner-api-openapi.yml
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
