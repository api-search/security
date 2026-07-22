---
api_specs:
- filename: virtru-authorization-openapi.yaml
  format: yaml
  label: Virtru Authorization (v1)
  slug: virtru-authorization-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-authorization-openapi.yaml
- filename: virtru-authorization-v2-openapi.yaml
  format: yaml
  label: Virtru Authorization (v2)
  slug: virtru-authorization-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-authorization-v2-openapi.yaml
- filename: virtru-entity-openapi.yaml
  format: yaml
  label: Virtru Entity
  slug: virtru-entity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-entity-openapi.yaml
- filename: virtru-entity-resolution-v2-openapi.yaml
  format: yaml
  label: Virtru Entity Resolution (v2)
  slug: virtru-entity-resolution-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-entity-resolution-v2-openapi.yaml
- filename: virtru-kas-openapi.yaml
  format: yaml
  label: Virtru Key Access Service (KAS)
  slug: virtru-key-access-service-kas
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-kas-openapi.yaml
- filename: virtru-policy-actions-openapi.yaml
  format: yaml
  label: Virtru Policy — Actions
  slug: virtru-policy-actions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-actions-openapi.yaml
- filename: virtru-policy-attributes-openapi.yaml
  format: yaml
  label: Virtru Policy — Attributes
  slug: virtru-policy-attributes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-attributes-openapi.yaml
- filename: virtru-policy-kas-registry-openapi.yaml
  format: yaml
  label: Virtru Policy — KAS Registry
  slug: virtru-policy-kas-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-kas-registry-openapi.yaml
- filename: virtru-policy-key-management-openapi.yaml
  format: yaml
  label: Virtru Policy — Key Management
  slug: virtru-policy-key-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-key-management-openapi.yaml
- filename: virtru-policy-namespaces-openapi.yaml
  format: yaml
  label: Virtru Policy — Namespaces
  slug: virtru-policy-namespaces
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-namespaces-openapi.yaml
- filename: virtru-policy-obligations-openapi.yaml
  format: yaml
  label: Virtru Policy — Obligations
  slug: virtru-policy-obligations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-obligations-openapi.yaml
- filename: virtru-policy-registered-resources-openapi.yaml
  format: yaml
  label: Virtru Policy — Registered Resources
  slug: virtru-policy-registered-resources
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-registered-resources-openapi.yaml
- filename: virtru-policy-resource-mapping-openapi.yaml
  format: yaml
  label: Virtru Policy — Resource Mapping
  slug: virtru-policy-resource-mapping
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-resource-mapping-openapi.yaml
- filename: virtru-policy-subject-mapping-openapi.yaml
  format: yaml
  label: Virtru Policy — Subject Mapping
  slug: virtru-policy-subject-mapping
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-subject-mapping-openapi.yaml
- filename: virtru-wellknown-configuration-openapi.yaml
  format: yaml
  label: Virtru Well-Known Configuration
  slug: virtru-well-known-configuration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-wellknown-configuration-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: virtru.com
  spf: true
hosts:
- cert_expires: Sep 29 17:29:21 2026 GMT
  host: www.virtru.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Virtru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Virtru, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Virtru
provider_slug: virtru
slug: virtru-domain-security
source_filename: virtru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.virtru.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 17:29:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: virtru.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/security/virtru-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Data Security
- Encryption
- Access Control
- Zero Trust
- Data Privacy
- OpenTDF
- Key Management
---
