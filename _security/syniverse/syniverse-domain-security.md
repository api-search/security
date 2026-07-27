---
api_specs:
- filename: syniverse-omni-channel-messaging-openapi.yml
  format: yaml
  label: Syniverse Omni-Channel Messaging API (SCG)
  slug: syniverse-omni-channel-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-omni-channel-messaging-openapi.yml
- filename: syniverse-multi-factor-authentication-openapi.yml
  format: yaml
  label: Syniverse Multi-Factor Authentication API
  slug: syniverse-multi-factor-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-multi-factor-authentication-openapi.yml
- filename: syniverse-phone-number-verification-openapi.yml
  format: yaml
  label: Syniverse Phone Number Verification API
  slug: syniverse-phone-number-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-phone-number-verification-openapi.yml
- filename: syniverse-right-party-verification-openapi.yml
  format: yaml
  label: Syniverse Right Party Verification API
  slug: syniverse-right-party-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-right-party-verification-openapi.yml
- filename: syniverse-account-takeover-detection-openapi.yml
  format: yaml
  label: Syniverse Account Takeover Detection API
  slug: syniverse-account-takeover-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-account-takeover-detection-openapi.yml
- filename: syniverse-messaging-trust-resolve-openapi.yml
  format: yaml
  label: Syniverse Messaging Trust Resolve API
  slug: syniverse-messaging-trust-resolve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-messaging-trust-resolve-openapi.yml
- filename: syniverse-messaging-trust-datafeed-openapi.yml
  format: yaml
  label: Syniverse Messaging Trust Spam Datafeed API
  slug: syniverse-messaging-trust-spam-datafeed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-messaging-trust-datafeed-openapi.yml
- filename: syniverse-10dlc-openapi.yml
  format: yaml
  label: Syniverse 10DLC API
  slug: syniverse-10dlc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-10dlc-openapi.yml
- filename: syniverse-10dlc-number-pool-openapi.yml
  format: yaml
  label: Syniverse 10DLC Number Pool API (v1, deprecated)
  slug: syniverse-10dlc-number-pool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-10dlc-number-pool-openapi.yml
- filename: syniverse-whitelisting-service-openapi.json
  format: json
  label: Syniverse Whitelisting Service API
  slug: syniverse-whitelisting-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-whitelisting-service-openapi.json
- filename: syniverse-token-management-openapi.yml
  format: yaml
  label: Syniverse SDC Application Access Token Management API
  slug: syniverse-access-token-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-token-management-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: syniverse.com
  spf: true
hosts:
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: www.syniverse.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: sdcdocumentation.syniverse.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: api.syniverse.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Syniverse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Syniverse, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Syniverse
provider_slug: syniverse
slug: syniverse-domain-security
source_filename: syniverse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.syniverse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sdcdocumentation.syniverse.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: false\n- host: api.syniverse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: syniverse.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/security/syniverse-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telecommunications
- United States
- CPaaS
- Messaging
- SMS
- Roaming
- IPX
- Wholesale
- Identity Verification
- SIM Swap
- 10DLC
- Open Gateway
- Network APIs
- Aggregator
---
