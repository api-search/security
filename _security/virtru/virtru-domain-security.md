---
api_specs:
- filename: virtru-authorization-authorizationservice-api-openapi.yml
  format: yaml
  label: Virtru authorization.AuthorizationService API
  slug: virtru-authorization-authorizationservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-authorization-authorizationservice-api-openapi.yml
- filename: virtru-authorization-v2-authorizationservice-api-openapi.yml
  format: yaml
  label: Virtru authorization.v2.AuthorizationService API
  slug: virtru-authorization-v2-authorizationservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-authorization-v2-authorizationservice-api-openapi.yml
- filename: virtru-entityresolution-v2-entityresolutionservice-api-openapi.yml
  format: yaml
  label: Virtru entityresolution.v2.EntityResolutionService API
  slug: virtru-entityresolution-v2-entityresolutionservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-entityresolution-v2-entityresolutionservice-api-openapi.yml
- filename: virtru-kas-accessservice-api-openapi.yml
  format: yaml
  label: Virtru kas.AccessService API
  slug: virtru-kas-accessservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-kas-accessservice-api-openapi.yml
- filename: virtru-policy-actions-actionservice-api-openapi.yml
  format: yaml
  label: Virtru policy.actions.ActionService API
  slug: virtru-policy-actions-actionservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-actions-actionservice-api-openapi.yml
- filename: virtru-policy-attributes-attributesservice-api-openapi.yml
  format: yaml
  label: Virtru policy.attributes.AttributesService API
  slug: virtru-policy-attributes-attributesservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-attributes-attributesservice-api-openapi.yml
- filename: virtru-policy-kasregistry-keyaccessserverregistryservice-api-openapi.yml
  format: yaml
  label: Virtru policy.kasregistry.KeyAccessServerRegistryService API
  slug: virtru-policy-kasregistry-keyaccessserverregistryservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-kasregistry-keyaccessserverregistryservice-api-openapi.yml
- filename: virtru-policy-keymanagement-keymanagementservice-api-openapi.yml
  format: yaml
  label: Virtru policy.keymanagement.KeyManagementService API
  slug: virtru-policy-keymanagement-keymanagementservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-keymanagement-keymanagementservice-api-openapi.yml
- filename: virtru-policy-namespaces-namespaceservice-api-openapi.yml
  format: yaml
  label: Virtru policy.namespaces.NamespaceService API
  slug: virtru-policy-namespaces-namespaceservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-namespaces-namespaceservice-api-openapi.yml
- filename: virtru-policy-obligations-service-api-openapi.yml
  format: yaml
  label: Virtru policy.obligations.Service API
  slug: virtru-policy-obligations-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-obligations-service-api-openapi.yml
- filename: virtru-policy-registeredresources-registeredresourcesservice-api-openapi.yml
  format: yaml
  label: Virtru policy.registeredresources.RegisteredResourcesService API
  slug: virtru-policy-registeredresources-registeredresourcesservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-registeredresources-registeredresourcesservice-api-openapi.yml
- filename: virtru-policy-resourcemapping-resourcemappingservice-api-openapi.yml
  format: yaml
  label: Virtru policy.resourcemapping.ResourceMappingService API
  slug: virtru-policy-resourcemapping-resourcemappingservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-resourcemapping-resourcemappingservice-api-openapi.yml
- filename: virtru-policy-subjectmapping-subjectmappingservice-api-openapi.yml
  format: yaml
  label: Virtru policy.subjectmapping.SubjectMappingService API
  slug: virtru-policy-subjectmapping-subjectmappingservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-subjectmapping-subjectmappingservice-api-openapi.yml
- filename: virtru-wellknownconfiguration-wellknownservice-api-openapi.yml
  format: yaml
  label: Virtru wellknownconfiguration.WellKnownService API
  slug: virtru-wellknownconfiguration-wellknownservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-wellknownconfiguration-wellknownservice-api-openapi.yml
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
