---
api_specs:
- filename: triodos-bank-uk-account-information-service-api-openapi.yml
  format: yaml
  label: Triodos Bank UK Account Information Service API
  slug: triodos-bank-uk-account-information-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/openapi/triodos-bank-uk-account-information-service-api-openapi.yml
- filename: triodos-bank-uk-authorization-endpoint-api-openapi.yml
  format: yaml
  label: Triodos Bank UK Authorization Endpoint API
  slug: triodos-bank-uk-authorization-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/openapi/triodos-bank-uk-authorization-endpoint-api-openapi.yml
- filename: triodos-bank-uk-client-registration-endpoint-api-openapi.yml
  format: yaml
  label: Triodos Bank UK Client Registration Endpoint API
  slug: triodos-bank-uk-client-registration-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/openapi/triodos-bank-uk-client-registration-endpoint-api-openapi.yml
- filename: triodos-bank-uk-configuration-endpoint-api-openapi.yml
  format: yaml
  label: Triodos Bank UK Configuration Endpoint API
  slug: triodos-bank-uk-configuration-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/openapi/triodos-bank-uk-configuration-endpoint-api-openapi.yml
- filename: triodos-bank-uk-confirmation-of-funds-service-api-openapi.yml
  format: yaml
  label: Triodos Bank UK Confirmation of Funds Service API
  slug: triodos-bank-uk-confirmation-of-funds-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/openapi/triodos-bank-uk-confirmation-of-funds-service-api-openapi.yml
- filename: triodos-bank-uk-extended-account-information-service-api-openapi.yml
  format: yaml
  label: Triodos Bank UK Extended Account Information Service API
  slug: triodos-bank-uk-extended-account-information-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/openapi/triodos-bank-uk-extended-account-information-service-api-openapi.yml
- filename: triodos-bank-uk-initial-access-token-service-api-openapi.yml
  format: yaml
  label: Triodos Bank UK Initial Access Token Service API
  slug: triodos-bank-uk-initial-access-token-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/openapi/triodos-bank-uk-initial-access-token-service-api-openapi.yml
- filename: triodos-bank-uk-payment-initiation-service-api-openapi.yml
  format: yaml
  label: Triodos Bank UK Payment Initiation Service API
  slug: triodos-bank-uk-payment-initiation-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/openapi/triodos-bank-uk-payment-initiation-service-api-openapi.yml
- filename: triodos-bank-uk-token-endpoint-api-openapi.yml
  format: yaml
  label: Triodos Bank UK Token Endpoint API
  slug: triodos-bank-uk-token-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/openapi/triodos-bank-uk-token-endpoint-api-openapi.yml
- filename: triodos-bank-uk-userinfo-endpoint-api-openapi.yml
  format: yaml
  label: Triodos Bank UK UserInfo Endpoint API
  slug: triodos-bank-uk-userinfo-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/openapi/triodos-bank-uk-userinfo-endpoint-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: triodos.co.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: triodos.com
  spf: true
hosts:
- cert_expires: Jan 10 10:36:45 2027 GMT
  host: www.triodos.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 12:57:57 2026 GMT
  host: developer.triodos.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 12:06:27 2026 GMT
  host: api-ma.triodos.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Triodos Bank Uk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Triodos Bank UK, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Triodos Bank UK
provider_slug: triodos-bank-uk
slug: triodos-bank-uk-domain-security
source_filename: triodos-bank-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.triodos.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 10:36:45 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.triodos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:57:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-ma.triodos.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 13 12:06:27 2026 GMT\n  hsts: null\ndomains:\n- domain: triodos.co.uk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: triodos.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/security/triodos-bank-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- XS2A
- Berlin Group
- United Kingdom
- Payments
- Account Information
- Confirmation of Funds
- Ethical Banking
- Sustainable Finance
- Specialist Lender
---
