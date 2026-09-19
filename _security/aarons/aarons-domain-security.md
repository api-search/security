---
api_specs:
- filename: aarons-authorizesession-api-openapi.yml
  format: yaml
  label: Aaron's Authorize Session API
  slug: aarons-authorizesession-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aarons/refs/heads/main/openapi/aarons-authorizesession-api-openapi.yml
- filename: aarons-autopaycustomerretry-api-openapi.yml
  format: yaml
  label: Aaron's Auto Pay Customer Retry API
  slug: aarons-autopaycustomerretry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aarons/refs/heads/main/openapi/aarons-autopaycustomerretry-api-openapi.yml
- filename: aarons-createtoken-api-openapi.yml
  format: yaml
  label: Aaron's Create Token API
  slug: aarons-createtoken-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aarons/refs/heads/main/openapi/aarons-createtoken-api-openapi.yml
- filename: aarons-fiservpostback-api-openapi.yml
  format: yaml
  label: Aaron's Fiserv Postback API
  slug: aarons-fiservpostback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aarons/refs/heads/main/openapi/aarons-fiservpostback-api-openapi.yml
- filename: aarons-memorybearertoken-api-openapi.yml
  format: yaml
  label: Aaron's Memory Bearer Token API
  slug: aarons-memorybearertoken-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aarons/refs/heads/main/openapi/aarons-memorybearertoken-api-openapi.yml
- filename: aarons-memorytokenguid-api-openapi.yml
  format: yaml
  label: Aaron's Memory Token Guid API
  slug: aarons-memorytokenguid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aarons/refs/heads/main/openapi/aarons-memorytokenguid-api-openapi.yml
- filename: aarons-ping-api-openapi.yml
  format: yaml
  label: Aaron's Ping API
  slug: aarons-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aarons/refs/heads/main/openapi/aarons-ping-api-openapi.yml
- filename: aarons-repayauthpostback-api-openapi.yml
  format: yaml
  label: Aaron's Repay Auth Postback API
  slug: aarons-repayauthpostback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aarons/refs/heads/main/openapi/aarons-repayauthpostback-api-openapi.yml
- filename: aarons-repaycardvaultpostback-api-openapi.yml
  format: yaml
  label: Aaron's Repay Card Vault Postback API
  slug: aarons-repaycardvaultpostback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aarons/refs/heads/main/openapi/aarons-repaycardvaultpostback-api-openapi.yml
- filename: aarons-savedeviceintelligence-api-openapi.yml
  format: yaml
  label: Aaron's Save Device Intelligence API
  slug: aarons-savedeviceintelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aarons/refs/heads/main/openapi/aarons-savedeviceintelligence-api-openapi.yml
- filename: aarons-savetoken-api-openapi.yml
  format: yaml
  label: Aaron's Save Token API
  slug: aarons-savetoken-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aarons/refs/heads/main/openapi/aarons-savetoken-api-openapi.yml
- filename: aarons-updatecustomerretrynotification-api-openapi.yml
  format: yaml
  label: Aaron's Update Customer Retry Notification API
  slug: aarons-updatecustomerretrynotification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aarons/refs/heads/main/openapi/aarons-updatecustomerretrynotification-api-openapi.yml
- filename: aarons-create-session-api-openapi.yml
  format: yaml
  label: Aaron's Create Session API
  slug: aarons-create-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aarons/refs/heads/main/openapi/aarons-create-session-api-openapi.yml
- filename: aarons-customer-data-api-openapi.yml
  format: yaml
  label: Aaron's CUSTOMER DATA API
  slug: aarons-customer-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aarons/refs/heads/main/openapi/aarons-customer-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aarons.com
  spf: true
hosts:
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: www.aarons.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: api.aarons.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: myaccount.aarons.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Aarons Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aaron''s, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Aaron's
provider_slug: aarons
slug: aarons-domain-security
source_filename: aarons-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aarons.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.aarons.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: null\n- host: myaccount.aarons.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aarons.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aarons/refs/heads/main/security/aarons-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Lease-to-Own
- Retail
- Furniture
- Electronics
- Appliances
- Consumer Finance
- Fortune 1000
---
