---
api_specs:
- filename: tmt-id-authenticate-api-openapi.yml
  format: yaml
  label: TMT ID Authenticate API
  slug: tmt-id-authenticate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-authenticate-api-openapi.yml
- filename: tmt-id-http-api-api-openapi.yml
  format: yaml
  label: TMT ID HTTP API
  slug: tmt-id-http-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-http-api-api-openapi.yml
- filename: tmt-id-http-api-v1-3-api-openapi.yml
  format: yaml
  label: TMT ID HTTP API v1.3 API
  slug: tmt-id-http-api-v1-3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-http-api-v1-3-api-openapi.yml
- filename: tmt-id-http-api-v2-0-api-openapi.yml
  format: yaml
  label: TMT ID HTTP API v2.0 API
  slug: tmt-id-http-api-v2-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-http-api-v2-0-api-openapi.yml
- filename: tmt-id-network-biometrics-api-openapi.yml
  format: yaml
  label: TMT ID Network Biometrics API
  slug: tmt-id-network-biometrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-network-biometrics-api-openapi.yml
- filename: tmt-id-service-api-openapi.yml
  format: yaml
  label: TMT ID Service API
  slug: tmt-id-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-service-api-openapi.yml
- filename: tmt-id-standard-api-call-api-openapi.yml
  format: yaml
  label: TMT ID Standard API Call API
  slug: tmt-id-standard-api-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-standard-api-call-api-openapi.yml
- filename: tmt-id-v2-deprecated-api-openapi.yml
  format: yaml
  label: TMT ID v2 (deprecated) API
  slug: tmt-id-v2-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/openapi/tmt-id-v2-deprecated-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: tmtid.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: tmtanalysis.com
  spf: true
hosts:
- cert_expires: Oct 19 21:46:21 2026 GMT
  host: tmtid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 13:56:12 2026 GMT
  host: viteza.tmtanalysis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: api.tmtverify.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tmt Id Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TMT ID, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: TMT ID
provider_slug: tmt-id
slug: tmt-id-domain-security
source_filename: tmt-id-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tmtid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 21:46:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: viteza.tmtanalysis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 13:56:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tmtverify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tmtid.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: tmtanalysis.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tmt-id/refs/heads/main/security/tmt-id-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Telecommunications
- United Kingdom
- Identity Verification
- Mobile Identity
- SIM Swap
- Anti-Fraud
- Number Intelligence
- Silent Network Authentication
- GSMA Open Gateway
- Network APIs
- ENUM
- KYC
---
