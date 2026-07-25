---
api_specs:
- filename: rescuegroups-org-animals-api-openapi.yml
  format: yaml
  label: RescueGroups.org Animals API
  slug: rescuegroups-org-animals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rescuegroups-org/refs/heads/main/openapi/rescuegroups-org-animals-api-openapi.yml
- filename: rescuegroups-org-authentication-api-openapi.yml
  format: yaml
  label: RescueGroups.org Authentication API
  slug: rescuegroups-org-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rescuegroups-org/refs/heads/main/openapi/rescuegroups-org-authentication-api-openapi.yml
- filename: rescuegroups-org-breeds-api-openapi.yml
  format: yaml
  label: RescueGroups.org Breeds API
  slug: rescuegroups-org-breeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rescuegroups-org/refs/heads/main/openapi/rescuegroups-org-breeds-api-openapi.yml
- filename: rescuegroups-org-colors-api-openapi.yml
  format: yaml
  label: RescueGroups.org Colors API
  slug: rescuegroups-org-colors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rescuegroups-org/refs/heads/main/openapi/rescuegroups-org-colors-api-openapi.yml
- filename: rescuegroups-org-organizations-api-openapi.yml
  format: yaml
  label: RescueGroups.org Organizations API
  slug: rescuegroups-org-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rescuegroups-org/refs/heads/main/openapi/rescuegroups-org-organizations-api-openapi.yml
- filename: rescuegroups-org-patterns-api-openapi.yml
  format: yaml
  label: RescueGroups.org Patterns API
  slug: rescuegroups-org-patterns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rescuegroups-org/refs/heads/main/openapi/rescuegroups-org-patterns-api-openapi.yml
- filename: rescuegroups-org-pet-lists-api-openapi.yml
  format: yaml
  label: RescueGroups.org Pet Lists API
  slug: rescuegroups-org-pet-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rescuegroups-org/refs/heads/main/openapi/rescuegroups-org-pet-lists-api-openapi.yml
- filename: rescuegroups-org-species-api-openapi.yml
  format: yaml
  label: RescueGroups.org Species API
  slug: rescuegroups-org-species-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rescuegroups-org/refs/heads/main/openapi/rescuegroups-org-species-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rescuegroups.org
  spf: true
hosts:
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: rescuegroups.org
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: api.rescuegroups.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: dev1-api.rescuegroups.org
  https: false
kind: domain-security
layout: security
method: probed
name: Rescuegroups Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RescueGroups.org, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RescueGroups.org
provider_slug: rescuegroups-org
slug: rescuegroups-org-domain-security
source_filename: rescuegroups-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rescuegroups.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: api.rescuegroups.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: null\n- host: dev1-api.rescuegroups.org\n  https: false\ndomains:\n- domain: rescuegroups.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rescuegroups-org/refs/heads/main/security/rescuegroups-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Animals
- Pet Adoption
- Rescue
- Animal Welfare
---
