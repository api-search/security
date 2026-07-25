---
api_specs:
- filename: simscale-geometry-api-openapi.yml
  format: yaml
  label: SimScale Geometry API
  slug: simscale-geometry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simscale/refs/heads/main/openapi/simscale-geometry-api-openapi.yml
- filename: simscale-mesh-operations-api-openapi.yml
  format: yaml
  label: SimScale Mesh Operations API
  slug: simscale-mesh-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simscale/refs/heads/main/openapi/simscale-mesh-operations-api-openapi.yml
- filename: simscale-projects-api-openapi.yml
  format: yaml
  label: SimScale Projects API
  slug: simscale-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simscale/refs/heads/main/openapi/simscale-projects-api-openapi.yml
- filename: simscale-reports-api-openapi.yml
  format: yaml
  label: SimScale Reports API
  slug: simscale-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simscale/refs/heads/main/openapi/simscale-reports-api-openapi.yml
- filename: simscale-simulation-runs-api-openapi.yml
  format: yaml
  label: SimScale Simulation Runs API
  slug: simscale-simulation-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simscale/refs/heads/main/openapi/simscale-simulation-runs-api-openapi.yml
- filename: simscale-simulations-api-openapi.yml
  format: yaml
  label: SimScale Simulations API
  slug: simscale-simulations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simscale/refs/heads/main/openapi/simscale-simulations-api-openapi.yml
- filename: simscale-storage-api-openapi.yml
  format: yaml
  label: SimScale Storage API
  slug: simscale-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simscale/refs/heads/main/openapi/simscale-storage-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issuewild "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: simscale.com
  spf: true
hosts:
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: www.simscale.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: api.simscale.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Simscale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SimScale, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SimScale
provider_slug: simscale
slug: simscale-domain-security
source_filename: simscale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.simscale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.simscale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: simscale.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simscale/refs/heads/main/security/simscale-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CAE
- CFD
- FEA
- Simulation
- Engineering
---
