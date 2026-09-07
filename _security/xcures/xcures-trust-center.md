---
api_specs:
- filename: xcures-patient-registry-api-openapi.yml
  format: yaml
  label: xCures Public API
  slug: xcures-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xcures/refs/heads/main/openapi/xcures-patient-registry-api-openapi.yml
certification_count: 0
certifications: []
description: ''
kind: trust-center
layout: security
name: Xcures Trust Center
name_suffix: Trust Center
overview: xCures maintains a public trust center covering its security and compliance posture.
provider_name: xCures
provider_slug: xcures
slug: xcures-trust-center
source_filename: xcures-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://xcures.com/trust/\nurl: https://xcures.com/trust/\nhttp_status: 200\ntitle: xCures trust & transparency\ntagline: What we strive for, how we measure it, and where to verify it.\nnote: >-\n  Upgraded from the automated probe, which detected the keywords \"SOC 2\", \"ISO 27001\" and \"HIPAA\" on this\n  page and attributed all three to xCures. Reading the page shows that is wrong for two of them: SOC 2\n  Type 2 and ISO 27001:2022 are AWS's, which xCures inherits controls from. The certification xCures\n  itself holds is HITRUST e1, which the keyword probe missed entirely. Attribution is corrected below.\ncertifications_held_by_xcures:\n  - name: HITRUST e1 Certification\n    scope: xCures Clinical Clarity Engine\n    status: certified\n    year: 2025\n    upgrade_in_progress: HITRUST i1 Certification (2026)\n    quote: >-\n      \"The xCures Clinical Clarity Engine is HITRUST e1 certified (in the process of being upgraded\
  \ to\n      HITRUST i1 Certification).\"\n  - name: HIPAA\n    scope: xCures and the Clinical Clarity Engine, operating as a business associate\n    status: compliant\n    validation: annual HIPAA evaluation plus assessments under the HITRUST certification program\ncertifications_inherited_from_aws:\n  attribution_warning: >-\n    NOT xCures certifications. The page states these are held by AWS, that xCures \"is able to inherit\n    selected AWS HITRUST r2 controls to include as evidence in xCures's HITRUST certification program\",\n    and that it \"periodically reviews the AWS ISO 27001 certification and SOC 2 attestation report\".\n    Attributing them to xCures overstates its posture.\n  certifications:\n    - name: HITRUST r2 Certification\n      holder: AWS\n    - name: ISO 27001:2022 Certification\n      holder: AWS\n    - name: SOC 2 Type 2 Attestation\n      holder: AWS\nsecurity_controls:\n  - control: Encryption\n    detail: In transit (TLS) and at rest\n  - control: Access\
  \ Controls\n    detail: RBAC with least-privilege and minimum-necessary principles, MFA, and SSO\n  - control: Audit Logging\n    detail: Immutable logs via AWS + Datadog, SIEM monitoring\n  - control: Data Deletion\n    detail: In accordance with contractual requirements\n  - control: Provenance / audit trail\n    detail: Full CRUD audit logs maintained across all data access and modification events\ndata_governance_standards:\n  - standard: FHIR R4\n    detail: All extracted data mapped to FHIR R4 resources for downstream interoperability\n  - standard: OHDSI / OMOP\n    detail: Concepts normalized to OHDSI Standardized Vocabularies (SNOMED, LOINC, RxNorm)\n  - standard: mCODE\n    detail: Oncology-specific data elements aligned to the HL7 Minimal Common Oncology Data Elements profile\n  - standard: HIPAA\n    detail: HIPAA compliant with annual HIPAA evaluation and HITRUST certification program\nai_model_validation:\n  note: >-\n    Unusual for this catalog and worth recording: xCures\
  \ publishes measured accuracy for the AI that\n    produces its API's output, with a stated method and a named limitation set. Most AI-in-the-loop\n    providers publish neither.\n  approaches:\n    - name: Schema-based extraction\n      detail: >-\n        NER + relation extraction over unstructured clinical documents into FHIR R4 and OHDSI-normalized\n        structured data, with linkage to source verbatim preserved per element.\n    - name: Checklist-based assertion\n      detail: >-\n        RAG over the full longitudinal record, returning structured outputs with source citations and\n        evidence-hierarchy rules to resolve conflicting documentation.\n  method: >-\n    Validated against clinically trained human reviewers; each field classified TP/TN/FP/FN with\n    third-reviewer arbitration on discrepancies; random 10% audit. Only explicitly stated, verifiable\n    extractions count as true positives — correct inferences not present verbatim are counted as errors.\n  deployment_threshold:\
  \ accuracy and precision >= 95% before an extractor or checklist enters production\n  published_results:\n    - extractor: Medications\n      accuracy: 95.7%\n      precision: 97.5%\n      recall: 95.0%\n      f1: 96.3%\n    - extractor: Surgical Procedures\n      accuracy: 96.6%\n      precision: 97.7%\n      recall: 98.8%\n      f1: 98.2%\n    - extractor: Cancer Diagnosis\n      accuracy: 98.2%\n      precision: 98.7%\n      recall: 99.4%\n      f1: 99.0%\n    - extractor: Lines of Therapy\n      accuracy: 97.0%\n      precision: 95.4%\n      recall: 99.8%\n      f1: 97.6%\n  results_caveat: >-\n    xCures states these are a retrospective analysis of a defined historical dataset and do not guarantee\n    future performance.\n  source_citation: >-\n    Stuhlmiller TJ et al. \"A Scalable Method for Validated Data Extraction from Electronic Health Records\n    with Large Language Models.\" Submitted for peer review, 2026. Full methods, supplemental tables and\n    raw counts available\
  \ on request.\n  stated_limitations:\n    - >-\n      OCR quality — accuracy of extraction from scanned or faxed documents depends on document quality;\n      degraded scans may introduce errors or omissions.\n    - >-\n      Semantic search coverage gaps — checklists and schema LLMs rely on semantic search and use only the\n      top N semantically matched documents, so relevant information in lower-ranked documents can be\n      missed.\n  version_control: Extraction models are version-controlled and support rollback; A/B testing guides refinement\ninfrastructure:\n  hosting: AWS\n  monitoring: AWS + Datadog, SIEM\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xcures/refs/heads/main/security/xcures-trust-center.yml
summary_line: trust center published
tags:
- Health
- Healthcare
- Medical Records
- Interoperability
- FHIR
- Oncology
- Real World Data
- Clinical Data
- Artificial Intelligence
- TEFCA
- Carequality
- Patient Data
- HITRUST
- HIPAA
trust_url: https://xcures.com/trust/
---
