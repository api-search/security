---
api_specs:
- filename: noms-brands-api-openapi.yml
  format: yaml
  label: Noms Brands API
  slug: noms-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noms/refs/heads/main/openapi/noms-brands-api-openapi.yml
- filename: noms-foodgroups-api-openapi.yml
  format: yaml
  label: Noms Food Groups API
  slug: noms-foodgroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noms/refs/heads/main/openapi/noms-foodgroups-api-openapi.yml
- filename: noms-foods-api-openapi.yml
  format: yaml
  label: Noms Foods API
  slug: noms-foods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noms/refs/heads/main/openapi/noms-foods-api-openapi.yml
- filename: noms-market-api-openapi.yml
  format: yaml
  label: Noms Market API
  slug: noms-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noms/refs/heads/main/openapi/noms-market-api-openapi.yml
- filename: noms-nutrients-api-openapi.yml
  format: yaml
  label: Noms Nutrients API
  slug: noms-nutrients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noms/refs/heads/main/openapi/noms-nutrients-api-openapi.yml
- filename: noms-usage-api-openapi.yml
  format: yaml
  label: Noms Usage API
  slug: noms-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noms/refs/heads/main/openapi/noms-usage-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: noms.sh
  spf: true
hosts:
- cert_expires: Dec 23 02:05:20 2026 GMT
  host: noms.sh
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Noms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Noms, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Noms
provider_slug: noms
slug: noms-domain-security
source_filename: noms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: noms.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 02:05:20 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: noms.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noms/refs/heads/main/security/noms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Nutrition
- Food
- Data
- Health
---
