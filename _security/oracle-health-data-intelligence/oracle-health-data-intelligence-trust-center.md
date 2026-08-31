---
api_specs:
- filename: oracle-health-data-intelligence-populations-api-openapi.yml
  format: yaml
  label: Oracle Health Data Intelligence Populations API
  slug: oracle-health-data-intelligence-populations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-health-data-intelligence/refs/heads/main/openapi/oracle-health-data-intelligence-populations-api-openapi.yml
certifications:
- HIPAA
- HITRUST CSF
- SOC 2
- ISO/IEC 27001
- FedRAMP
- PCI DSS
description: Trust and compliance surface available to an Oracle Health Data Intelligence buyer. Oracle publishes a corporate cloud-compliance registry naming the attestations it holds. There is no product-scoped trust center for Health Data Intelligence, and no artifact request portal is linked from the developer documentation.
kind: trust-center
layout: security
name: Oracle Health Data Intelligence Trust Center
name_suffix: Trust Center
overview: Oracle Health Data Intelligence maintains a public trust center documenting HIPAA, HITRUST CSF, SOC 2, ISO/IEC 27001, FedRAMP, and PCI DSS compliance.
provider_name: Oracle Health Data Intelligence
provider_slug: oracle-health-data-intelligence
slug: oracle-health-data-intelligence-trust-center
source_filename: oracle-health-data-intelligence-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://www.oracle.com/corporate/cloud-compliance/\ndocs: https://www.oracle.com/corporate/cloud-compliance/\ndescription: >-\n  Trust and compliance surface available to an Oracle Health Data Intelligence buyer. Oracle\n  publishes a corporate cloud-compliance registry naming the attestations it holds. There is no\n  product-scoped trust center for Health Data Intelligence, and no artifact request portal is\n  linked from the developer documentation.\ntrust_center:\n  published: true\n  scope: corporate\n  url: https://www.oracle.com/corporate/cloud-compliance/\n  probed_status: 200\n  observed: '2026-08-27'\n  secondary_url: https://www.oracle.com/trust/\n  secondary_probed_status: 200\n  secondary_note: >-\n    oracle.com/trust renders client-side; no certification name is present in the served HTML, so\n    the compliance registry above is the readable source.\ncertifications:\n  - name: HIPAA\n    scope: Oracle cloud services\n\
  \    evidence: named in the Oracle cloud-compliance registry\n  - name: HITRUST CSF\n    scope: Oracle cloud services\n    evidence: named in the Oracle cloud-compliance registry\n  - name: SOC 2\n    scope: Oracle cloud services\n    evidence: named in the Oracle cloud-compliance registry\n  - name: ISO/IEC 27001\n    scope: Oracle cloud services\n    evidence: named in the Oracle cloud-compliance registry\n  - name: FedRAMP\n    scope: Oracle US government cloud regions\n    evidence: named in the Oracle cloud-compliance registry\n  - name: PCI DSS\n    scope: Oracle cloud services\n    evidence: named in the Oracle cloud-compliance registry\ngaps:\n  - >-\n    No Health Data Intelligence-specific attestation scope statement. A buyer cannot tell from\n    public material which of the corporate certifications cover this platform's regions and\n    services.\n  - No self-serve artifact request portal (no Whistic, Vanta, Drata or equivalent).\n  - No subprocessor list or data-residency\
  \ page linked from the developer portal.\n  - >-\n    Data residency is nonetheless material here: the platform is deployed as Oracle Cerner Cloud\n    Regions (us-1, emea-1, emea-2, ca-1, ap-1) and the region is part of the API hostname, so\n    residency is observable from the base URL even though it is not documented as a compliance\n    control.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-health-data-intelligence/refs/heads/main/security/oracle-health-data-intelligence-trust-center.yml
summary_line: HIPAA, HITRUST CSF, SOC 2, ISO/IEC 27001, FedRAMP, PCI DSS
tags:
- Genomic
- Health Records
- Healthcare
- Population Health
- Longitudinal Record
- Interoperability
- Clinical Data
- Analytics
trust_url: ''
---
