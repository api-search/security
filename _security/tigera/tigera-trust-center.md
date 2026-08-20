---
api_specs:
- filename: tigera-apis-api-openapi.yml
  format: yaml
  label: Tigera APIS API
  slug: tigera-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigera/refs/heads/main/openapi/tigera-apis-api-openapi.yml
- filename: tigera-projectcalicoorg-api-openapi.yml
  format: yaml
  label: Tigera Projectcalico Org API
  slug: tigera-projectcalicoorg-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigera/refs/heads/main/openapi/tigera-projectcalicoorg-api-openapi.yml
- filename: tigera-projectcalicoorg-v3-api-openapi.yml
  format: yaml
  label: Tigera Projectcalico Org V3 API
  slug: tigera-projectcalicoorg-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigera/refs/heads/main/openapi/tigera-projectcalicoorg-v3-api-openapi.yml
- filename: tigera-version-api-openapi.yml
  format: yaml
  label: Tigera Version API
  slug: tigera-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tigera/refs/heads/main/openapi/tigera-version-api-openapi.yml
certifications:
- CSA STAR
- SOC 2
- PCI DSS
- GDPR
- CCPA
description: Tigera publishes a Calico Cloud trust center page on the marketing site rather than a third-party trust portal (there is no trust.tigera.io — the host does not resolve). It names the compliance frameworks Calico Cloud is assessed against and points at the Cloud Security Alliance STAR registry entry for Tigera, Inc. Penetration-test reports are available to customers on request rather than published.
kind: trust-center
layout: security
name: Tigera Trust Center
name_suffix: Trust Center
overview: Tigera maintains a public trust center documenting CSA STAR, SOC 2, PCI DSS, GDPR, and CCPA compliance.
provider_name: Tigera
provider_slug: tigera
slug: tigera-trust-center
source_filename: tigera-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nprobe: true\nsource: https://www.tigera.io/tigera-products/calico-cloud-trust-center/\ndescription: >-\n  Tigera publishes a Calico Cloud trust center page on the marketing site rather than a\n  third-party trust portal (there is no trust.tigera.io — the host does not resolve). It names\n  the compliance frameworks Calico Cloud is assessed against and points at the Cloud Security\n  Alliance STAR registry entry for Tigera, Inc. Penetration-test reports are available to\n  customers on request rather than published.\nurl: https://www.tigera.io/tigera-products/calico-cloud-trust-center/\ncertifications:\n- name: CSA STAR\n  status: registered\n  evidence: https://cloudsecurityalliance.org/star/registry/tigera-inc\n- name: SOC 2\n  status: claimed\n  evidence: https://www.tigera.io/tigera-products/calico-cloud-trust-center/\n- name: PCI DSS\n  status: claimed\n  scope: payment processing system\n  evidence: https://www.tigera.io/tigera-products/calico-cloud-trust-center/\n\
  - name: GDPR\n  status: claimed\n  evidence: https://www.tigera.io/tigera-products/calico-cloud-trust-center/\n- name: CCPA\n  status: claimed\n  evidence: https://www.tigera.io/tigera-products/calico-cloud-trust-center/\npractices:\n- Encryption of data in transit (end to end)\n- Encryption of customer information at rest\n- RBAC and token-based authentication\n- Annual third-party penetration testing; reports available to customers on request\nreports:\n  self_service_portal: false\n  request_required: true\n  note: >-\n    No automated NDA/report-request workflow (no Vanta/Drata/SafeBase-style portal). Reports are\n    obtained through the sales or support channel.\nvulnerability_disclosure: security/tigera-vulnerability-disclosure.yml\nprobed:\n- url: https://trust.tigera.io/\n  status: 0\n  reason: dns-nxdomain\n- url: https://www.tigera.io/trust/\n  status: 404\n- url: https://www.tigera.io/tigera-products/calico-cloud-trust-center/\n  status: 200\nx-evidence:\n  fetched: '2026-08-05'\n\
  \  url: https://www.tigera.io/tigera-products/calico-cloud-trust-center/\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tigera/refs/heads/main/security/tigera-trust-center.yml
summary_line: CSA STAR, SOC 2, PCI DSS, GDPR, CCPA
tags:
- Company
- Kubernetes
- Networking
- Network Security
- Container Security
- Cloud-Native
- Observability
- Microsegmentation
- Zero Trust
- eBPF
- Open-Source
trust_url: https://www.tigera.io/tigera-products/calico-cloud-trust-center/
---
