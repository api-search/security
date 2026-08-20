---
api_specs:
- filename: bluecore-authn-api-openapi.yml
  format: yaml
  label: Bluecore Authn API
  slug: bluecore-authn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/openapi/bluecore-authn-api-openapi.yml
- filename: bluecore-campaignsapipublic-api-openapi.yml
  format: yaml
  label: Bluecore CampaignsAPIPublic API
  slug: bluecore-campaignsapipublic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/openapi/bluecore-campaignsapipublic-api-openapi.yml
- filename: bluecore-direct-send-api-openapi.yml
  format: yaml
  label: Bluecore Direct send API
  slug: bluecore-direct-send-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/openapi/bluecore-direct-send-api-openapi.yml
- filename: bluecore-eligibility-api-openapi.yml
  format: yaml
  label: Bluecore Eligibility API
  slug: bluecore-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/openapi/bluecore-eligibility-api-openapi.yml
- filename: bluecore-profile-api-openapi.yml
  format: yaml
  label: Bluecore Profile API
  slug: bluecore-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/openapi/bluecore-profile-api-openapi.yml
- filename: bluecore-transactional-api-openapi.yml
  format: yaml
  label: Bluecore Transactional API
  slug: bluecore-transactional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/openapi/bluecore-transactional-api-openapi.yml
- filename: bluecore-transactional-legacy-api-openapi.yml
  format: yaml
  label: Bluecore Transactional API (legacy)
  slug: bluecore-transactional-legacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/openapi/bluecore-transactional-legacy-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: bluecore.com
  spf: true
hosts:
- cert_expires: Sep 28 02:55:48 2026 GMT
  host: bluecore.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 21:03:16 2026 GMT
  host: developers.bluecore.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 17:38:17 2026 GMT
  host: a.bluecore.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bluecore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bluecore, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Bluecore
provider_slug: bluecore
slug: bluecore-domain-security
source_filename: bluecore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bluecore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 02:55:48 2026 GMT\n  hsts: false\n- host: developers.bluecore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 21:03:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: a.bluecore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 17:38:17 2026 GMT\n  hsts: null\ndomains:\n- domain: bluecore.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/security/bluecore-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Retail
- Marketing
- Customer Data Platform
- Personalization
- Email
- SMS
- Messaging
- E-Commerce
- Consent
---
