---
api_specs:
- filename: voltair-apikeys-api-openapi.yml
  format: yaml
  label: Voltair ApiKeys API
  slug: voltair-apikeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-apikeys-api-openapi.yml
- filename: voltair-assets-api-openapi.yml
  format: yaml
  label: Voltair Assets API
  slug: voltair-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-assets-api-openapi.yml
- filename: voltair-clusters-api-openapi.yml
  format: yaml
  label: Voltair Clusters API
  slug: voltair-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-clusters-api-openapi.yml
- filename: voltair-clustervisits-api-openapi.yml
  format: yaml
  label: Voltair ClusterVisits API
  slug: voltair-clustervisits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-clustervisits-api-openapi.yml
- filename: voltair-events-api-openapi.yml
  format: yaml
  label: Voltair Events API
  slug: voltair-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-events-api-openapi.yml
- filename: voltair-identity-api-openapi.yml
  format: yaml
  label: Voltair Identity API
  slug: voltair-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-identity-api-openapi.yml
- filename: voltair-inspections-api-openapi.yml
  format: yaml
  label: Voltair Inspections API
  slug: voltair-inspections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-inspections-api-openapi.yml
- filename: voltair-media-api-openapi.yml
  format: yaml
  label: Voltair Media API
  slug: voltair-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-media-api-openapi.yml
- filename: voltair-missions-api-openapi.yml
  format: yaml
  label: Voltair Missions API
  slug: voltair-missions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-missions-api-openapi.yml
- filename: voltair-organization-api-openapi.yml
  format: yaml
  label: Voltair Organization API
  slug: voltair-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-organization-api-openapi.yml
- filename: voltair-roles-api-openapi.yml
  format: yaml
  label: Voltair Roles API
  slug: voltair-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-roles-api-openapi.yml
- filename: voltair-sites-api-openapi.yml
  format: yaml
  label: Voltair Sites API
  slug: voltair-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-sites-api-openapi.yml
- filename: voltair-sitevisits-api-openapi.yml
  format: yaml
  label: Voltair SiteVisits API
  slug: voltair-sitevisits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-sitevisits-api-openapi.yml
- filename: voltair-transactions-api-openapi.yml
  format: yaml
  label: Voltair Transactions API
  slug: voltair-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-transactions-api-openapi.yml
- filename: voltair-users-api-openapi.yml
  format: yaml
  label: Voltair Users API
  slug: voltair-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-users-api-openapi.yml
- filename: voltair-webhooks-api-openapi.yml
  format: yaml
  label: Voltair Webhooks API
  slug: voltair-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/openapi/voltair-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: voltairlabs.com
  spf: true
hosts:
- cert_expires: Sep 30 15:21:12 2026 GMT
  host: voltairlabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: api.voltairlabs.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Voltair Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voltair, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Voltair
provider_slug: voltair
slug: voltair-domain-security
source_filename: voltair-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: voltairlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 15:21:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.voltairlabs.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: voltairlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voltair/refs/heads/main/security/voltair-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Drones
- Earth Observation
- Infrastructure Inspection
- Utilities
- Energy
- Robotics
- LiDAR
- Aerial Imagery
---
