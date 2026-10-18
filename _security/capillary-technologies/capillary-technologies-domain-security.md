---
api_specs:
- filename: capillary-technologies-events-api-openapi.yml
  format: yaml
  label: Capillary Technologies Events API
  slug: capillary-technologies-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capillary-technologies/refs/heads/main/openapi/capillary-technologies-events-api-openapi.yml
- filename: capillary-technologies-simulation-api-openapi.yml
  format: yaml
  label: Capillary Technologies Simulation API
  slug: capillary-technologies-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capillary-technologies/refs/heads/main/openapi/capillary-technologies-simulation-api-openapi.yml
- filename: capillary-technologies-webhooks-api-openapi.yml
  format: yaml
  label: Capillary Technologies Webhooks API
  slug: capillary-technologies-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capillary-technologies/refs/heads/main/openapi/capillary-technologies-webhooks-api-openapi.yml
- filename: capillary-technologies-x-api-openapi.yml
  format: yaml
  label: Capillary Technologies X API
  slug: capillary-technologies-x-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capillary-technologies/refs/heads/main/openapi/capillary-technologies-x-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: capillarytech.com
  spf: true
hosts:
- cert_expires: Nov 10 17:57:31 2026 GMT
  host: www.capillarytech.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Capillary Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capillary Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Capillary Technologies
provider_slug: capillary-technologies
slug: capillary-technologies-domain-security
source_filename: capillary-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.capillarytech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 17:57:31 2026 GMT\n  hsts: null\ndomains:\n- domain: capillarytech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capillary-technologies/refs/heads/main/security/capillary-technologies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Loyalty
- Marketing
- Software-as-a-Service
- Enterprise
- Customer-Engagement
---
