---
api_specs:
- filename: fiware-api-entry-point-api-openapi.yml
  format: yaml
  label: FIWARE API Entry Point API
  slug: fiware-api-entry-point-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiware/refs/heads/main/openapi/fiware-api-entry-point-api-openapi.yml
- filename: fiware-attribute-value-api-openapi.yml
  format: yaml
  label: FIWARE Attribute Value API
  slug: fiware-attribute-value-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiware/refs/heads/main/openapi/fiware-attribute-value-api-openapi.yml
- filename: fiware-attributes-api-openapi.yml
  format: yaml
  label: FIWARE Attributes API
  slug: fiware-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiware/refs/heads/main/openapi/fiware-attributes-api-openapi.yml
- filename: fiware-batch-operations-api-openapi.yml
  format: yaml
  label: FIWARE Batch Operations API
  slug: fiware-batch-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiware/refs/heads/main/openapi/fiware-batch-operations-api-openapi.yml
- filename: fiware-context-information-api-openapi.yml
  format: yaml
  label: FIWARE Context Information API
  slug: fiware-context-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiware/refs/heads/main/openapi/fiware-context-information-api-openapi.yml
- filename: fiware-context-sources-api-openapi.yml
  format: yaml
  label: FIWARE Context Sources API
  slug: fiware-context-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiware/refs/heads/main/openapi/fiware-context-sources-api-openapi.yml
- filename: fiware-context-subscription-api-openapi.yml
  format: yaml
  label: FIWARE Context Subscription API
  slug: fiware-context-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiware/refs/heads/main/openapi/fiware-context-subscription-api-openapi.yml
- filename: fiware-entities-api-openapi.yml
  format: yaml
  label: FIWARE Entities API
  slug: fiware-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiware/refs/heads/main/openapi/fiware-entities-api-openapi.yml
- filename: fiware-registrations-api-openapi.yml
  format: yaml
  label: FIWARE Registrations API
  slug: fiware-registrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiware/refs/heads/main/openapi/fiware-registrations-api-openapi.yml
- filename: fiware-subscriptions-api-openapi.yml
  format: yaml
  label: FIWARE Subscriptions API
  slug: fiware-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiware/refs/heads/main/openapi/fiware-subscriptions-api-openapi.yml
- filename: fiware-temporal-evolution-api-openapi.yml
  format: yaml
  label: FIWARE Temporal Evolution API
  slug: fiware-temporal-evolution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiware/refs/heads/main/openapi/fiware-temporal-evolution-api-openapi.yml
- filename: fiware-types-api-openapi.yml
  format: yaml
  label: FIWARE Types API
  slug: fiware-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiware/refs/heads/main/openapi/fiware-types-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fiware.org
  spf: true
hosts:
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: www.fiware.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: orion.lab.fiware.org
  https: false
kind: domain-security
layout: security
method: probed
name: Fiware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FIWARE, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FIWARE
provider_slug: fiware
slug: fiware-domain-security
source_filename: fiware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fiware.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: false\n- host: orion.lab.fiware.org\n  https: false\ndomains:\n- domain: fiware.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fiware/refs/heads/main/security/fiware-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Context Information
- Devices
- Internet of Things
- Linked Data
- NGSI
- Smart Cities
- Standards
---
