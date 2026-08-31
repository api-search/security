---
api_specs:
- filename: cutiss-newsroom-api-openapi.yml
  format: yaml
  label: CUTISS Newsroom API
  slug: cutiss-newsroom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cutiss/refs/heads/main/openapi/cutiss-newsroom-api-openapi.yml
- filename: cutiss-posts-api-openapi.yml
  format: yaml
  label: CUTISS Posts API
  slug: cutiss-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cutiss/refs/heads/main/openapi/cutiss-posts-api-openapi.yml
- filename: cutiss-pages-api-openapi.yml
  format: yaml
  label: CUTISS Pages API
  slug: cutiss-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cutiss/refs/heads/main/openapi/cutiss-pages-api-openapi.yml
- filename: cutiss-team-api-openapi.yml
  format: yaml
  label: CUTISS Team API
  slug: cutiss-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cutiss/refs/heads/main/openapi/cutiss-team-api-openapi.yml
- filename: cutiss-media-api-openapi.yml
  format: yaml
  label: CUTISS Media API
  slug: cutiss-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cutiss/refs/heads/main/openapi/cutiss-media-api-openapi.yml
- filename: cutiss-categories-api-openapi.yml
  format: yaml
  label: CUTISS Categories API
  slug: cutiss-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cutiss/refs/heads/main/openapi/cutiss-categories-api-openapi.yml
- filename: cutiss-search-api-openapi.yml
  format: yaml
  label: CUTISS Search API
  slug: cutiss-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cutiss/refs/heads/main/openapi/cutiss-search-api-openapi.yml
- filename: cutiss-teams-taxonomy-api-openapi.yml
  format: yaml
  label: CUTISS Teams Taxonomy API
  slug: cutiss-teams-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cutiss/refs/heads/main/openapi/cutiss-teams-taxonomy-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cutiss.swiss
  spf: true
hosts:
- cert_expires: Sep 15 09:46:05 2026 GMT
  host: cutiss.swiss
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cutiss Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CUTISS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CUTISS
provider_slug: cutiss
slug: cutiss-domain-security
source_filename: cutiss-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cutiss.swiss\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 09:46:05 2026 GMT\n  hsts: false\ndomains:\n- domain: cutiss.swiss\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cutiss/refs/heads/main/security/cutiss-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Regenerative Medicine
- Tissue Engineering
- Life Sciences
- Medical Devices
- Clinical Trials
- Dermatology
- Healthcare
- Switzerland
- Research
- Content
---
