---
api_specs:
- filename: ocean-health-systems-archetypes-api-openapi.yml
  format: yaml
  label: Ocean Health Systems Archetypes API
  slug: ocean-health-systems-archetypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-health-systems/refs/heads/main/openapi/ocean-health-systems-archetypes-api-openapi.yml
- filename: ocean-health-systems-change-requests-api-openapi.yml
  format: yaml
  label: Ocean Health Systems Change Requests API
  slug: ocean-health-systems-change-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-health-systems/refs/heads/main/openapi/ocean-health-systems-change-requests-api-openapi.yml
- filename: ocean-health-systems-projects-api-openapi.yml
  format: yaml
  label: Ocean Health Systems Projects API
  slug: ocean-health-systems-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-health-systems/refs/heads/main/openapi/ocean-health-systems-projects-api-openapi.yml
- filename: ocean-health-systems-resource-proposals-api-openapi.yml
  format: yaml
  label: Ocean Health Systems Resource Proposals API
  slug: ocean-health-systems-resource-proposals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-health-systems/refs/heads/main/openapi/ocean-health-systems-resource-proposals-api-openapi.yml
- filename: ocean-health-systems-resources-api-openapi.yml
  format: yaml
  label: Ocean Health Systems Resources API
  slug: ocean-health-systems-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-health-systems/refs/heads/main/openapi/ocean-health-systems-resources-api-openapi.yml
- filename: ocean-health-systems-sessions-api-openapi.yml
  format: yaml
  label: Ocean Health Systems Sessions API
  slug: ocean-health-systems-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-health-systems/refs/heads/main/openapi/ocean-health-systems-sessions-api-openapi.yml
- filename: ocean-health-systems-subdomains-api-openapi.yml
  format: yaml
  label: Ocean Health Systems Subdomains API
  slug: ocean-health-systems-subdomains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-health-systems/refs/heads/main/openapi/ocean-health-systems-subdomains-api-openapi.yml
- filename: ocean-health-systems-templates-api-openapi.yml
  format: yaml
  label: Ocean Health Systems Templates API
  slug: ocean-health-systems-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-health-systems/refs/heads/main/openapi/ocean-health-systems-templates-api-openapi.yml
- filename: ocean-health-systems-users-api-openapi.yml
  format: yaml
  label: Ocean Health Systems Users API
  slug: ocean-health-systems-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-health-systems/refs/heads/main/openapi/ocean-health-systems-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: oceanhealthsystems.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: openehr.org
  spf: true
hosts:
- cert_expires: Nov 20 11:00:41 2026 GMT
  host: oceanhealthsystems.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 19:15:14 2026 GMT
  host: ckm.openehr.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Ocean Health Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ocean Health Systems, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ocean Health Systems
provider_slug: ocean-health-systems
slug: ocean-health-systems-domain-security
source_filename: ocean-health-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oceanhealthsystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 11:00:41 2026 GMT\n  hsts: false\n- host: ckm.openehr.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 19:15:14 2026 GMT\n  hsts: false\ndomains:\n- domain: oceanhealthsystems.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: openehr.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ocean-health-systems/refs/heads/main/security/ocean-health-systems-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Health
- Healthcare
- Electronic Health Records
- openEHR
- Clinical Data
- Clinical Knowledge Management
- Interoperability
- Health Informatics
- Terminology
- Archetypes
- Infection Prevention
- immunisation
---
