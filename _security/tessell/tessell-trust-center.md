---
api_specs:
- filename: tessell-openapi-original.json
  format: json
  label: Tessell API
  slug: tessell-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tessell/refs/heads/main/openapi/tessell-openapi-original.json
certifications:
- PCI DSS v4.1
- SOC 2
- ISO 27001
- ISO/IEC 27701
description: Tessell publishes its security and compliance posture on a dedicated "Security and Compliance" platform page rather than a trust.<domain> portal. The page names the certifications it holds, states FedRAMP status explicitly, and describes the sovereignty architecture (data plane in the customer's own cloud account with BYOA/BYOK). The standard trust-center hostnames (trust.tessell.com, security.tessell.com) do not resolve.
kind: trust-center
layout: security
name: Tessell Trust Center
name_suffix: Trust Center
overview: Tessell maintains a public trust center documenting PCI DSS v4.1, SOC 2, ISO 27001, and ISO/IEC 27701 compliance.
provider_name: Tessell
provider_slug: tessell
slug: tessell-trust-center
source_filename: tessell-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nprobe: false\nsource: https://www.tessell.com/platform/security-and-compliance\nurl: https://www.tessell.com/platform/security-and-compliance\ndescription: >-\n  Tessell publishes its security and compliance posture on a dedicated \"Security and Compliance\"\n  platform page rather than a trust.<domain> portal. The page names the certifications it holds,\n  states FedRAMP status explicitly, and describes the sovereignty architecture (data plane in the\n  customer's own cloud account with BYOA/BYOK). The standard trust-center hostnames\n  (trust.tessell.com, security.tessell.com) do not resolve.\ncertifications:\n- PCI DSS v4.1\n- SOC 2\n- ISO 27001\n- ISO/IEC 27701\nstatements:\n- >-\n  \"Tessell is an independently verified holder of PCI DSS v4.1, SOC 2, ISO 27001, and ISO 27701.\"\n- >-\n  \"Is Tessell FedRAMP authorized? Tessell is not FedRAMP authorized.\" (Tessell positions BYOA\n  deployment inside the customer's own authorized\
  \ cloud boundary instead.)\n- >-\n  SOC 2 Type II attestation announced with zero exceptions noted\n  (https://www.tessell.com/blogs/tessell-soc2-type2).\nevidence:\n- source: https://www.tessell.com/platform/security-and-compliance\n  keywords: [PCI DSS v4.1, SOC 2, ISO 27001, ISO/IEC 27701, FedRAMP, certifications and attestations]\n- source: https://www.tessell.com/blogs/tessell-soc2-type2\n  keywords: [SOC 2 Type II]\nrelated:\n- type: SecurityPage\n  url: https://www.tessell.com/platform/security\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tessell/refs/heads/main/security/tessell-trust-center.yml
summary_line: PCI DSS v4.1, SOC 2, ISO 27001, ISO/IEC 27701
tags:
- Databases
- DBaaS
- Multi-Cloud
- Oracle
- PostgreSQL
- MySQL
- SQL Server
- Data Infrastructure
trust_url: https://www.tessell.com/platform/security-and-compliance
---
