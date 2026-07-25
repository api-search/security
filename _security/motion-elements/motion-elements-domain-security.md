---
api_specs:
- filename: motion-elements-account-api-openapi.yml
  format: yaml
  label: Motion Elements Account API
  slug: motion-elements-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/motion-elements/refs/heads/main/openapi/motion-elements-account-api-openapi.yml
- filename: motion-elements-elements-api-openapi.yml
  format: yaml
  label: Motion Elements Elements API
  slug: motion-elements-elements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/motion-elements/refs/heads/main/openapi/motion-elements-elements-api-openapi.yml
- filename: motion-elements-media-types-api-openapi.yml
  format: yaml
  label: Motion Elements Media types API
  slug: motion-elements-media-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/motion-elements/refs/heads/main/openapi/motion-elements-media-types-api-openapi.yml
- filename: motion-elements-search-api-openapi.yml
  format: yaml
  label: Motion Elements Search API
  slug: motion-elements-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/motion-elements/refs/heads/main/openapi/motion-elements-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: motionelements.com
  spf: true
hosts:
- cert_expires: Oct 18 03:55:37 2026 GMT
  host: motionelements.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 07:20:57 2026 GMT
  host: api.motionelements.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Motion Elements Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Motion Elements, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Motion Elements
provider_slug: motion-elements
slug: motion-elements-domain-security
source_filename: motion-elements-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: motionelements.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 03:55:37 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: api.motionelements.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 07:20:57 2026 GMT\n  hsts: null\ndomains:\n- domain: motionelements.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/motion-elements/refs/heads/main/security/motion-elements-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Media
- Stock Media
- Video
- Music
- Sound Effects
- Templates
- Marketplace
- Creative Assets
- Generative AI
- Search
- Company
---
