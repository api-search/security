---
certifications:
- SOC 2 Type 1
- SOC 2 Type 2
- ISO/IEC 27001
description: ''
kind: trust-center
layout: security
name: Granica Trust Center
name_suffix: Trust Center
overview: Granica maintains a public trust center documenting SOC 2 Type 1, SOC 2 Type 2, and ISO/IEC 27001 compliance.
provider_name: Granica
provider_slug: granica
slug: granica-trust-center
source_filename: granica-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: searched\nsource: https://docs.granica.ai/security-and-compliance/security-certifications\nnote: >-\n  Granica publishes no separate trust.granica.ai portal. Its compliance disclosure lives in the public\n  documentation, on the Security certifications page, which names specific attestations and the process for\n  requesting the reports. That page is the trust surface and is what this artifact points at.\ntrust_center_url: https://docs.granica.ai/security-and-compliance/security-certifications\ndedicated_portal: false\ncertifications:\n- name: SOC 2 Type 1\n  status: current\n  auditor: independent CBA-registered CPA firm\n  evidence: 'Listed under \"Current\" on the security certifications page.'\n  report_availability: >-\n    Restricted. Shared only with prospective customers under NDA or current customers bound by\n    confidentiality agreements. Requested from security@granica.ai with company name, requestor name, email\n    and job title;\
  \ acknowledgement within one business day.\n- name: SOC 2 Type 2\n  status: current\n  auditor: independent CBA-registered CPA firm\n  evidence: 'Listed under \"Current\" on the security certifications page.'\n  report_availability: Same restricted NDA process as the Type 1 report.\n- name: ISO/IEC 27001\n  status: planned\n  evidence: 'Listed under \"Planned (Roadmap)\".'\nregimes:\n- name: HIPAA\n  posture: conditional / architecture-compatible\n  statement: >-\n    Granica does not directly handle protected health information. Data stays within the customer's own\n    HIPAA-compliant cloud environment, Granica relies on the cloud provider's native encryption at rest and\n    in transit, the control plane runs within the customer's VPC, and data isolation follows the customer's\n    per-tenant bucket layout. Granica states it \"can be part of an overall HIPAA-compliant architecture\"\n    rather than claiming certification.\ncontacts:\n- purpose: security and compliance report requests\n\
  \  email: security@granica.ai\ndata_residency:\n  models:\n  - name: Granica Hosted\n    data_leaves_customer_cloud: table data and catalog metadata\n  - name: On-Premises (2A, with tunnel)\n    data_leaves_customer_cloud: Console HTML, aggregated reports and metrics, table names and metadata, policies, activity stats, configuration\n  - name: On-Premises (2B, without tunnel)\n    data_leaves_customer_cloud: none\n  - name: Hybrid\n    data_leaves_customer_cloud: Spark job progress, job status, failures and performance metrics\n  source: https://docs.granica.ai/installation/deployment-models\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/granica/refs/heads/main/security/granica-trust-center.yml
summary_line: SOC 2 Type 1, SOC 2 Type 2, ISO/IEC 27001
tags:
- Company
- Data
- Storage
- Analytics
- Artificial Intelligence
- Machine-Learning
- Data Lakehouse
- Cloud Cost Optimization
- Compression
- Data Infrastructure
trust_url: ''
---
