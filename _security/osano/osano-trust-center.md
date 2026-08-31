---
api_specs:
- filename: osano-cmp-api-openapi.yml
  format: yaml
  label: Osano Cmp API
  slug: osano-cmp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-cmp-api-openapi.yml
- filename: osano-cmprules-api-openapi.yml
  format: yaml
  label: Osano Cmp Rules API
  slug: osano-cmprules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-cmprules-api-openapi.yml
- filename: osano-collections-api-openapi.yml
  format: yaml
  label: Osano Collections API
  slug: osano-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-collections-api-openapi.yml
- filename: osano-config-api-openapi.yml
  format: yaml
  label: Osano Config API
  slug: osano-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-config-api-openapi.yml
- filename: osano-connectors-api-openapi.yml
  format: yaml
  label: Osano Connectors API
  slug: osano-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-connectors-api-openapi.yml
- filename: osano-consent-profiles-api-openapi.yml
  format: yaml
  label: Osano Consent Profiles API
  slug: osano-consent-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-consent-profiles-api-openapi.yml
- filename: osano-consents-api-openapi.yml
  format: yaml
  label: Osano Consents API
  slug: osano-consents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-consents-api-openapi.yml
- filename: osano-customerinsights-api-openapi.yml
  format: yaml
  label: Osano Customer Insights API
  slug: osano-customerinsights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-customerinsights-api-openapi.yml
- filename: osano-datadiscovery-api-openapi.yml
  format: yaml
  label: Osano Data Discovery API
  slug: osano-datadiscovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-datadiscovery-api-openapi.yml
- filename: osano-dsar-api-openapi.yml
  format: yaml
  label: Osano Dsar API
  slug: osano-dsar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-dsar-api-openapi.yml
- filename: osano-dsaractionitems-api-openapi.yml
  format: yaml
  label: Osano Dsar Action Items API
  slug: osano-dsaractionitems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-dsaractionitems-api-openapi.yml
- filename: osano-sessions-api-openapi.yml
  format: yaml
  label: Osano Sessions API
  slug: osano-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-sessions-api-openapi.yml
- filename: osano-subjectrightsportal-api-openapi.yml
  format: yaml
  label: Osano Subject Rights Portal API
  slug: osano-subjectrightsportal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-subjectrightsportal-api-openapi.yml
- filename: osano-subjects-api-openapi.yml
  format: yaml
  label: Osano Subjects API
  slug: osano-subjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-subjects-api-openapi.yml
- filename: osano-token-api-openapi.yml
  format: yaml
  label: Osano Token API
  slug: osano-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-token-api-openapi.yml
- filename: osano-unified-consent-core-api-api-openapi.yml
  format: yaml
  label: Osano Unified Consent Core API
  slug: osano-unified-consent-core-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-unified-consent-core-api-api-openapi.yml
certifications:
- SOC 2
- Enterprise audit package
description: ''
kind: trust-center
layout: security
name: Osano Trust Center
name_suffix: Trust Center
overview: Osano maintains a public trust center documenting SOC 2 and Enterprise audit package compliance.
provider_name: Osano
provider_slug: osano
slug: osano-trust-center
source_filename: osano-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://trust.osano.com/ and https://www.osano.com/faq\nevidence:\n- url: https://trust.osano.com/\n  status: 200\n  detail: >-\n    Vanta-hosted trust center, canonical https://trust.osano.com, title \"Osano Trust Center\",\n    description \"At Osano, we take your privacy seriously. This Trust Center is designed to share\n    information that enables you to get information about how we handle data and how we will work\n    with you.\" Listed in Osano's own llms.txt under Optional.\n- url: https://trust.osano.com/subprocessors\n  status: 200\n- url: https://www.osano.com/faq\n  status: 200\ntrust_center:\n  url: https://trust.osano.com/\n  platform: Vanta\n  machine_readable: false\n  note: >-\n    The trust center is a client-rendered Vanta application; the certification list, document\n    requests and subprocessor table are fetched by JavaScript, so no certification names could be\n    read from the served HTML. The certification\
  \ claims below are quoted from Osano's OWN FAQ page,\n    which does serve them as text. Nothing here is inferred from the Vanta shell.\ncertifications:\n- name: SOC 2\n  status: maintained\n  evidence_verbatim: >-\n    \"Osano maintains an always current SOC2 report which is available upon request to customers on\n    any paid plan.\"\n  source: https://www.osano.com/faq\n  public_report: false\n  note: Report is gated behind a paid-customer request; type (I/II) is not stated on the public page.\n- name: Enterprise audit package\n  status: available-on-request\n  evidence_verbatim: >-\n    \"If you are a current or prospective Enterprise customer, Osano can provide a full suite of\n    third-party audits, policies, documentation, code security reports, code coverage reports, and\n    architectural walkthroughs for your security team assessments.\"\n  source: https://www.osano.com/faq\nsecurity_practices:\n- practice: vulnerability-scanning\n  evidence_verbatim: 'Osano infrastructure and\
  \ systems are tested for vulnerabilities nightly'\n  source: https://www.osano.com/faq\n- practice: penetration-testing\n  evidence_verbatim: 'are routinely penetration tested'\n  source: https://www.osano.com/faq\n- practice: encryption\n  evidence_verbatim: >-\n    \"all data is transferred (in transit) and stored (at rest) using modern encryption protocols such\n    as TLS1.3 and AES 256 respectively\"\n  source: https://www.osano.com/faq\n- practice: per-customer-key-separation\n  evidence_verbatim: >-\n    \"Personal data is encrypted using an encryption key which is unique to each customer. Most data\n    is stored using a per customer salt and SHA-512 hashing.\"\n  source: https://www.osano.com/faq\n- practice: eu-data-residency\n  evidence_verbatim: >-\n    \"Osano stores de-identified data in our Dublin, Ireland data center and does not store\n    identifiable information about your visitors, nor do we transfer personal data outside of the\n    European Economic Area.\"\n  source:\
  \ https://www.osano.com/faq\ncorporate_status:\n- 'Certified B Corporation (per Osano llms.txt and www.osano.com/company/about)'\n- 'Public Benefit Corporation — the GitHub organization is registered as \"Osano, Inc., A Public Benefit Corporation\"'\nnot_found:\n  iso_27001: Not named on any public Osano page reached in this pass.\n  pci_dss: Not named.\n  hipaa: Not named.\n  fedramp: Not named.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/security/osano-trust-center.yml
summary_line: SOC 2, Enterprise audit package
tags:
- Company
- Data Privacy
- Consent Management
- Compliance
- GDPR
- CCPA
- Cookie Consent
- Subject Rights
- Data Mapping
- Vendor Risk
- Privacy Assessments
- Governance Risk Compliance
trust_url: ''
---
