---
api_specs:
- filename: calico-bgpconfiguration-api-openapi.yml
  format: yaml
  label: Calico BGPConfiguration API
  slug: calico-bgpconfiguration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calico/refs/heads/main/openapi/calico-bgpconfiguration-api-openapi.yml
- filename: calico-bgppeer-api-openapi.yml
  format: yaml
  label: Calico BGPPeer API
  slug: calico-bgppeer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calico/refs/heads/main/openapi/calico-bgppeer-api-openapi.yml
- filename: calico-globalnetworkpolicy-api-openapi.yml
  format: yaml
  label: Calico GlobalNetworkPolicy API
  slug: calico-globalnetworkpolicy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calico/refs/heads/main/openapi/calico-globalnetworkpolicy-api-openapi.yml
- filename: calico-hostendpoint-api-openapi.yml
  format: yaml
  label: Calico HostEndpoint API
  slug: calico-hostendpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calico/refs/heads/main/openapi/calico-hostendpoint-api-openapi.yml
- filename: calico-ippool-api-openapi.yml
  format: yaml
  label: Calico IPPool API
  slug: calico-ippool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calico/refs/heads/main/openapi/calico-ippool-api-openapi.yml
- filename: calico-networkpolicy-api-openapi.yml
  format: yaml
  label: Calico NetworkPolicy API
  slug: calico-networkpolicy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calico/refs/heads/main/openapi/calico-networkpolicy-api-openapi.yml
- filename: calico-profile-api-openapi.yml
  format: yaml
  label: Calico Profile API
  slug: calico-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calico/refs/heads/main/openapi/calico-profile-api-openapi.yml
certification_count: 5
certifications:
- SOC 2
- Cloud Security Alliance (CSA)
- GDPR
- CCPA
- PCI DSS
description: ''
kind: trust-center
layout: security
name: Calico Trust Center
name_suffix: Trust Center
overview: Calico maintains a public trust center documenting SOC 2, Cloud Security Alliance (CSA), GDPR, CCPA, and PCI DSS compliance.
provider_name: Calico
provider_slug: calico
slug: calico-trust-center
source_filename: calico-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://www.tigera.io/tigera-products/calico-cloud-trust-center/\nurl: https://www.tigera.io/tigera-products/calico-cloud-trust-center/\nhttp_status: 200\nname: Calico Cloud Trust Center\noperator: Tigera, Inc.\nscope: >-\n  Applies to CALICO CLOUD, the hosted commercial edition. Calico Open Source is Apache-2.0 software\n  the operator runs in its own cluster — it holds no certification and needs none.\ncertifications:\n- name: SOC 2\n  status: claimed\n  quote: '\"Calico Cloud is SOC 2, CCPA, GDPR compliant\"'\n  type_level: not stated — the page does not distinguish Type I from Type II\n  report_access: on request\n- name: Cloud Security Alliance (CSA)\n  status: claimed\n  quote: '\"Calico Cloud is certified with Cloud Security Alliance\"'\n  report_access: CSA STAR registry\n- name: GDPR\n  status: claimed\n  quote: '\"Calico Cloud is SOC 2, CCPA, GDPR compliant\"'\n- name: CCPA\n  status: claimed\n  quote: '\"Calico Cloud\
  \ is SOC 2, CCPA, GDPR compliant\"'\n- name: PCI DSS\n  status: claimed-with-caveat\n  quote: '\"Our payment processing system is PCI compliant\"'\n  caveat: >-\n    Reads as the BILLING system, not the Calico Cloud platform. Not promoted to a platform\n    certification here.\nsecurity_practices:\n- encryption_in_transit: '\"end-to-end encryption for data in transit\"'\n- encryption_at_rest: '\"customer information is encrypted at rest\"'\n- authentication: '\"supports RBAC and Token based authentication\"'\n- penetration_testing: '\"perform yearly PEN test to ensure compliance and the report is available to customers upon request\"'\nreport_access:\n  self_serve_portal: false\n  mechanism: on request\n  note: >-\n    No automated report-request portal, NDA flow or document vault. SOC 2 and pen-test reports are\n    \"available upon request\", which means a human loop.\ngaps:\n- No ISO 27001 claim found.\n- No FedRAMP claim found.\n- No published sub-processor list.\n- No published data-residency\
  \ statement.\n- >-\n  The page does not separate what Tigera itself is certified for from what Calico helps CUSTOMERS\n  achieve. Frameworks Calico markets as customer-enablement (PCI DSS, HIPAA, NIST, custom) are\n  deliberately excluded from the certifications list above.\nrelated:\n  conformance: conformance/calico-conformance.yml\n  vulnerability_disclosure: security/calico-vulnerability-disclosure.yml\n  security_bulletins: https://www.tigera.io/security-bulletins/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calico/refs/heads/main/security/calico-trust-center.yml
summary_line: SOC 2, Cloud Security Alliance (CSA), GDPR, CCPA, PCI DSS
tags:
- CNI
- Containers
- eBPF
- Kubernetes
- Network Policy
- Network Security
- Networking
- Open-Source
- Service Mesh
trust_url: https://www.tigera.io/tigera-products/calico-cloud-trust-center/
---
