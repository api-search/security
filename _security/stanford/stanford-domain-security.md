---
api_specs:
- filename: stanford-about-api-openapi.yml
  format: yaml
  label: Stanford University About API
  slug: stanford-about-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-about-api-openapi.yml
- filename: stanford-authentication-api-openapi.yml
  format: yaml
  label: Stanford University Authentication API
  slug: stanford-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-authentication-api-openapi.yml
- filename: stanford-catalog-api-openapi.yml
  format: yaml
  label: Stanford University Catalog API
  slug: stanford-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-catalog-api-openapi.yml
- filename: stanford-events-api-openapi.yml
  format: yaml
  label: Stanford University Events API
  slug: stanford-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-events-api-openapi.yml
- filename: stanford-files-api-openapi.yml
  format: yaml
  label: Stanford University Files API
  slug: stanford-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-files-api-openapi.yml
- filename: stanford-identifiers-api-openapi.yml
  format: yaml
  label: Stanford University Identifiers API
  slug: stanford-identifiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-identifiers-api-openapi.yml
- filename: stanford-integrations-api-openapi.yml
  format: yaml
  label: Stanford University Integrations API
  slug: stanford-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-integrations-api-openapi.yml
- filename: stanford-jobs-api-openapi.yml
  format: yaml
  label: Stanford University Jobs API
  slug: stanford-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-jobs-api-openapi.yml
- filename: stanford-legacy-api-openapi.yml
  format: yaml
  label: Stanford University Legacy API
  slug: stanford-legacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-legacy-api-openapi.yml
- filename: stanford-metadata-api-openapi.yml
  format: yaml
  label: Stanford University Metadata API
  slug: stanford-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-metadata-api-openapi.yml
- filename: stanford-objects-api-openapi.yml
  format: yaml
  label: Stanford University Objects API
  slug: stanford-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-objects-api-openapi.yml
- filename: stanford-release-tags-api-openapi.yml
  format: yaml
  label: Stanford University Release Tags API
  slug: stanford-release-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-release-tags-api-openapi.yml
- filename: stanford-tags-api-openapi.yml
  format: yaml
  label: Stanford University Tags API
  slug: stanford-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-tags-api-openapi.yml
- filename: stanford-versions-api-openapi.yml
  format: yaml
  label: Stanford University Versions API
  slug: stanford-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-versions-api-openapi.yml
- filename: stanford-workflows-api-openapi.yml
  format: yaml
  label: Stanford University Workflows API
  slug: stanford-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-workflows-api-openapi.yml
- filename: stanford-workspaces-api-openapi.yml
  format: yaml
  label: Stanford University Workspaces API
  slug: stanford-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-workspaces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: stanford.edu
  spf: true
hosts:
- cert_expires: Sep 23 14:19:11 2026 GMT
  host: www.stanford.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 10:53:43 2026 GMT
  host: api.library.stanford.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: purl.stanford.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Stanford Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stanford University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Stanford University
provider_slug: stanford
slug: stanford-domain-security
source_filename: stanford-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stanford.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 14:19:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.library.stanford.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 10:53:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: purl.stanford.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stanford.edu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/security/stanford-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- University
- Higher Education
- Education
- Research
- United States
- California
- Private Research University
- Association of American Universities
- Research Repository
- Course Catalog
- Identity Federation
- Library
- Digital Repository
- Artificial Intelligence
- IIIF
---
