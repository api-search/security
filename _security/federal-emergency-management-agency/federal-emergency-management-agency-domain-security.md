---
api_specs:
- filename: federal-emergency-management-agency-assistance-api-openapi.yml
  format: yaml
  label: Federal Emergency Management Agency Assistance API
  slug: federal-emergency-management-agency-assistance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-emergency-management-agency/refs/heads/main/openapi/federal-emergency-management-agency-assistance-api-openapi.yml
- filename: federal-emergency-management-agency-disasters-api-openapi.yml
  format: yaml
  label: Federal Emergency Management Agency Disasters API
  slug: federal-emergency-management-agency-disasters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-emergency-management-agency/refs/heads/main/openapi/federal-emergency-management-agency-disasters-api-openapi.yml
- filename: federal-emergency-management-agency-metadata-api-openapi.yml
  format: yaml
  label: Federal Emergency Management Agency Metadata API
  slug: federal-emergency-management-agency-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-emergency-management-agency/refs/heads/main/openapi/federal-emergency-management-agency-metadata-api-openapi.yml
- filename: federal-emergency-management-agency-nfip-api-openapi.yml
  format: yaml
  label: Federal Emergency Management Agency NFIP API
  slug: federal-emergency-management-agency-nfip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-emergency-management-agency/refs/heads/main/openapi/federal-emergency-management-agency-nfip-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fema.gov
  spf: true
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.fema.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Federal Emergency Management Agency Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Federal Emergency Management Agency, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Federal Emergency Management Agency
provider_slug: federal-emergency-management-agency
slug: federal-emergency-management-agency-domain-security
source_filename: federal-emergency-management-agency-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fema.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: fema.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-emergency-management-agency/refs/heads/main/security/federal-emergency-management-agency-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Disasters
- Emergencies
- Federal Government
- Flood Insurance
- Hazard Mitigation
---
