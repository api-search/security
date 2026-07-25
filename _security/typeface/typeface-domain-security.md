---
api_specs:
- filename: typeface-audiences-api-openapi.yml
  format: yaml
  label: Typeface Audiences API
  slug: typeface-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-audiences-api-openapi.yml
- filename: typeface-authentication-api-openapi.yml
  format: yaml
  label: Typeface Authentication API
  slug: typeface-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-authentication-api-openapi.yml
- filename: typeface-basic-services-api-openapi.yml
  format: yaml
  label: Typeface Basic Services API
  slug: typeface-basic-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-basic-services-api-openapi.yml
- filename: typeface-brand-kits-api-openapi.yml
  format: yaml
  label: Typeface Brand Kits API
  slug: typeface-brand-kits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-brand-kits-api-openapi.yml
- filename: typeface-content-generation-api-openapi.yml
  format: yaml
  label: Typeface Content Generation API
  slug: typeface-content-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-content-generation-api-openapi.yml
- filename: typeface-content-service-api-openapi.yml
  format: yaml
  label: Typeface Content Service API
  slug: typeface-content-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-content-service-api-openapi.yml
- filename: typeface-digital-assets-api-openapi.yml
  format: yaml
  label: Typeface Digital Assets API
  slug: typeface-digital-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-digital-assets-api-openapi.yml
- filename: typeface-discovery-api-openapi.yml
  format: yaml
  label: Typeface Discovery API
  slug: typeface-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-discovery-api-openapi.yml
- filename: typeface-feeds-api-openapi.yml
  format: yaml
  label: Typeface Feeds API
  slug: typeface-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-feeds-api-openapi.yml
- filename: typeface-profile-service-api-openapi.yml
  format: yaml
  label: Typeface Profile Service API
  slug: typeface-profile-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-profile-service-api-openapi.yml
- filename: typeface-projects-api-openapi.yml
  format: yaml
  label: Typeface Projects API
  slug: typeface-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-projects-api-openapi.yml
- filename: typeface-provisioning-api-openapi.yml
  format: yaml
  label: Typeface Provisioning API
  slug: typeface-provisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-provisioning-api-openapi.yml
- filename: typeface-provisioning-service-api-openapi.yml
  format: yaml
  label: Typeface Provisioning Service API
  slug: typeface-provisioning-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-provisioning-service-api-openapi.yml
- filename: typeface-search-service-api-openapi.yml
  format: yaml
  label: Typeface Search Service API
  slug: typeface-search-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-search-service-api-openapi.yml
- filename: typeface-tag-library-api-openapi.yml
  format: yaml
  label: Typeface Tag Library API
  slug: typeface-tag-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-tag-library-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: typeface.ai
  spf: true
hosts:
- cert_expires: Oct  9 01:18:28 2026 GMT
  host: www.typeface.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 05:51:39 2026 GMT
  host: api-us.typeface.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Typeface Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Typeface, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Typeface
provider_slug: typeface
slug: typeface-domain-security
source_filename: typeface-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.typeface.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 01:18:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-us.typeface.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 05:51:39 2026 GMT\n  hsts: null\ndomains:\n- domain: typeface.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/security/typeface-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Artificial Intelligence
- Content Generation
- Marketing
- Agents
- Generative AI
- Brand Management
- Enterprise
---
