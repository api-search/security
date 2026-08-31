---
api_specs:
- filename: scale-computing-api-keys-api-openapi.yml
  format: yaml
  label: Scale Computing API Keys API
  slug: scale-computing-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-api-keys-api-openapi.yml
- filename: scale-computing-clusters-api-openapi.yml
  format: yaml
  label: Scale Computing Clusters API
  slug: scale-computing-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-clusters-api-openapi.yml
- filename: scale-computing-conditions-api-openapi.yml
  format: yaml
  label: Scale Computing Conditions API
  slug: scale-computing-conditions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-conditions-api-openapi.yml
- filename: scale-computing-health-api-openapi.yml
  format: yaml
  label: Scale Computing Health API
  slug: scale-computing-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-health-api-openapi.yml
- filename: scale-computing-metrics-api-openapi.yml
  format: yaml
  label: Scale Computing Metrics API
  slug: scale-computing-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-metrics-api-openapi.yml
- filename: scale-computing-nodes-api-openapi.yml
  format: yaml
  label: Scale Computing Nodes API
  slug: scale-computing-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-nodes-api-openapi.yml
- filename: scale-computing-organization-activities-api-openapi.yml
  format: yaml
  label: Scale Computing Organization Activities API
  slug: scale-computing-organization-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-organization-activities-api-openapi.yml
- filename: scale-computing-organization-api-openapi.yml
  format: yaml
  label: Scale Computing Organization API
  slug: scale-computing-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-organization-api-openapi.yml
- filename: scale-computing-organization-salesforce-account-api-openapi.yml
  format: yaml
  label: Scale Computing Organization Salesforce Account API
  slug: scale-computing-organization-salesforce-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-organization-salesforce-account-api-openapi.yml
- filename: scale-computing-organizationroles-api-openapi.yml
  format: yaml
  label: Scale Computing Organization Roles API
  slug: scale-computing-organizationroles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-organizationroles-api-openapi.yml
- filename: scale-computing-organizations-api-openapi.yml
  format: yaml
  label: Scale Computing Organizations API
  slug: scale-computing-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-organizations-api-openapi.yml
- filename: scale-computing-organizationuser-api-openapi.yml
  format: yaml
  label: Scale Computing Organization User API
  slug: scale-computing-organizationuser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-organizationuser-api-openapi.yml
- filename: scale-computing-organizationusers-api-openapi.yml
  format: yaml
  label: Scale Computing Organization Users API
  slug: scale-computing-organizationusers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-organizationusers-api-openapi.yml
- filename: scale-computing-salesforce-api-openapi.yml
  format: yaml
  label: Scale Computing Salesforce API
  slug: scale-computing-salesforce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-salesforce-api-openapi.yml
- filename: scale-computing-staged-clusters-api-openapi.yml
  format: yaml
  label: Scale Computing Staged Clusters API
  slug: scale-computing-staged-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-staged-clusters-api-openapi.yml
- filename: scale-computing-users-api-openapi.yml
  format: yaml
  label: Scale Computing Users API
  slug: scale-computing-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-users-api-openapi.yml
- filename: scale-computing-vms-api-openapi.yml
  format: yaml
  label: Scale Computing Vms API
  slug: scale-computing-vms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-vms-api-openapi.yml
certifications: []
description: ''
kind: trust-center
layout: security
name: Scale Computing Trust Center
name_suffix: Trust Center
overview: Scale Computing maintains a public trust center covering its security and compliance posture.
provider_name: Scale Computing
provider_slug: scale-computing
slug: scale-computing-trust-center
source_filename: scale-computing-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://www.scalecomputing.com/security\ntrust_center:\n  published: false\n  url: null\n  note: >-\n    No trust center found. trust.scalecomputing.com does not serve a page (Cloudflare edge answers the\n    hostname with a challenge to a raw client and returns HTTP 404 to a browser-agent fetch), and\n    www.scalecomputing.com/security is a product-marketing page, not a compliance portal.\ncertifications: []\nx-false-positive-correction:\n  detected_by: 0-working/probe-security-programs.py\n  detected: [SOC 2, PCI DSS]\n  verdict: rejected\n  reason: >-\n    The keyword probe matched \"SOC 2\" and \"PCI DSS\" on https://www.scalecomputing.com/security, but on\n    reading the page those strings appear in offerings Scale Computing sells TO customers (\"PCI DSS\n    Compliance Solutions for Secure, Scalable Payment Environments\", a free PCI assessment tool, and a\n    white paper titled \"Enabling Regulatory Compliance with\
  \ Your IT Infrastructure Platform\"). The page\n    makes no claim that Scale Computing itself holds a SOC 2 attestation or a PCI DSS certification, and\n    no such claim was found elsewhere on the site. Recorded as absent rather than credited.\n  checked: '2026-08-26'\nevidence:\n- url: https://www.scalecomputing.com/security\n  status: 200\n  finding: marketing page; compliance offerings for customers, no self-attestation\n- url: https://trust.scalecomputing.com\n  status: 404\n  finding: no trust center served (403 Cloudflare challenge to curl, 404 to a browser-agent fetch)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/security/scale-computing-trust-center.yml
summary_line: trust center published
tags:
- edge-computing
- hyperconverged-infrastructure
- Virtualization
- infrastructure-management
- fleet-management
- virtual-machines
- observability
- infrastructure-as-code
- kubernetes
trust_url: ''
---
