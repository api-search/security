---
api_specs:
- filename: crowdtwist-starter-kit.postman_collection.json
  format: json
  label: Oracle CrowdTwist Loyalty and Engagement API
  slug: crowdtwist-loyalty
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/crowdtwist/refs/heads/main/postman/crowdtwist-starter-kit.postman_collection.json
certifications: []
description: ''
kind: trust-center
layout: security
name: Crowdtwist Trust Center
name_suffix: Trust Center
overview: CrowdTwist maintains a public trust center covering its security and compliance posture.
provider_name: CrowdTwist
provider_slug: crowdtwist
slug: crowdtwist-trust-center
source_filename: crowdtwist-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://www.oracle.com/corporate/cloud-compliance/\napi: Oracle CrowdTwist Loyalty and Engagement\nsummary: >-\n  There is no CrowdTwist trust center. The trust surface for this product is Oracle's corporate\n  Cloud Compliance program, which is the correct owner under the parent-brand rule — Oracle\n  acquired CrowdTwist in March 2019, sells it as an Oracle Cloud Service under the Oracle Cloud\n  Hosting and Delivery Policies, and the Service Descriptions document explicitly subjects a\n  CrowdTwist order to \"the Oracle Cloud Hosting and Delivery Policies and the Oracle SaaS Public\n  Cloud Services pillar documentation\".\ntrust_center:\n  published: true\n  owner: Oracle Corporation (parent)\n  url: https://www.oracle.com/corporate/cloud-compliance/\n  http_status: 200\n  fetched: '2026-08-13'\n  contracts_hub: https://www.oracle.com/contracts\n  security_practices: https://www.oracle.com/corporate/security-practices/\n\
  programs_named_on_the_page:\n- SOC 1\n- SOC 2\n- SOC 3\n- ISO/IEC 27001\n- ISO/IEC 27017\n- ISO/IEC 27018\n- PCI DSS\n- HIPAA\n- FedRAMP\n- CSA STAR\n- C5\n- IRAP\nscope_caveat: >-\n  IMPORTANT — these are the programs Oracle names across its cloud portfolio, not certifications\n  attested for Oracle CrowdTwist Loyalty and Engagement. Oracle publishes no per-service scope\n  statement naming CrowdTwist, and CrowdTwist does not appear on any attestation listing we could\n  reach without a login. Nothing here should be read as \"CrowdTwist is FedRAMP authorized\".\ncrowdtwist_specific:\n  certifications_published: false\n  service_description: https://www.oracle.com/contracts/docs/corporate_crowdtwist_cloud_service_descriptions_090320.pdf\n  service_description_effective: '2024-09-12'\n  published_commitments:\n    target_service_availability: 99.8%\n    rto: 72 hours\n    rpo: 24 hours\n    data_residency: >-\n      Global Data Center Region option allows deployment in any eligible Oracle\
  \ cloud region;\n      dedicated DE (Germany) and US2 production environments are documented on the API endpoint\n      reference page.\n  privacy_controls_in_product:\n  - member delete endpoint (DELETE /v2/users/{user_id})\n  - PII-minimised member creation (POST /v2/users?pii=false)\n  - COPPA date-of-birth validation\npointer_note: >-\n  A `TrustCenter` pointer is wired in apis.yml. A `Compliance` pointer deliberately is NOT — the\n  certifications above are Oracle-wide, and asserting them for CrowdTwist would credit this\n  product with attestations whose scope its own vendor does not publish.\nlegal:\n  terms_of_service: https://www.oracle.com/legal/terms/\n  privacy_policy: https://www.oracle.com/legal/privacy/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowdtwist/refs/heads/main/security/crowdtwist-trust-center.yml
summary_line: trust center published
tags:
- Company
- Loyalty
- Customer Engagement
- Marketing
- Gamification
- Rewards
- Oracle
- CX Marketing
- Loyalty Programs
- Points
- Retail
- Commerce
- Segmentation
- Webhooks
trust_url: ''
---
