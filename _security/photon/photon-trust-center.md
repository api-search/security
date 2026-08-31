---
api_specs:
- filename: photon-agent-discovery-api-openapi.yml
  format: yaml
  label: Photon Agent discovery API
  slug: photon-agent-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photon/refs/heads/main/openapi/photon-agent-discovery-api-openapi.yml
- filename: photon-newsletter-api-openapi.yml
  format: yaml
  label: Photon Newsletter API
  slug: photon-newsletter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photon/refs/heads/main/openapi/photon-newsletter-api-openapi.yml
- filename: photon-onboarding-api-openapi.yml
  format: yaml
  label: Photon Onboarding API
  slug: photon-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/photon/refs/heads/main/openapi/photon-onboarding-api-openapi.yml
certifications:
- SOC 2
- HIPAA
description: ''
kind: trust-center
layout: security
name: Photon Trust Center
name_suffix: Trust Center
overview: Photon maintains a public trust center documenting SOC 2 and HIPAA compliance.
provider_name: Photon
provider_slug: photon
slug: photon-trust-center
source_filename: photon-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://trust.photon.health + https://photonhealth.com/faq + https://photonhealth.com/baa\ntrust_center:\n  url: https://trust.photon.health\n  status: 200\n  platform: Vanta\n  slug: cw5vz8j1xq7tausfpowe\n  machine_readable: false\n  note: >-\n    The trust center is a Vanta-hosted single-page app. The shell returns HTTP\n    200 with the title \"Photon Trust Center\" but every control, certification\n    and subprocessor is rendered client-side, so no certification list can be\n    read from the served HTML. The certifications recorded below therefore come\n    from Photon's own first-party pages, not from scraping the trust center.\ncertifications:\n- name: SOC 2\n  status: claimed\n  evidence: >-\n    \"Yes, Photon is HIPAA & SOC-2 compliant.\" - published verbatim on\n    https://photonhealth.com/faq (HTTP 200), under \"Is Photon HIPAA compliant?\".\n  source: https://photonhealth.com/faq\n  report_available: unknown\n\
  \  note: Type (I vs II) is not stated on any public page; the report itself is behind the Vanta trust center.\n- name: HIPAA\n  status: claimed\n  evidence: >-\n    Same FAQ answer; reinforced by a published Platform Business Associate\n    Agreement covering HIPAA and the HITECH Act.\n  source: https://photonhealth.com/faq\nregulatory_posture:\n- framework: HIPAA / HITECH\n  role: Business Associate\n  artifact: https://photonhealth.com/baa\n  status: 200\n  last_updated: '2025-10-14'\n  note: >-\n    Photon Health, Inc. publishes a click-accept Platform Business Associate\n    Agreement, incorporated by reference into the Order Form, naming itself\n    Business Associate to covered-entity customers. A published BAA is the\n    strongest HIPAA signal a vendor can serve without an audit report.\n- framework: Controlled substances (EPCS)\n  status: out-of-scope\n  evidence: 'FAQ: \"Does Photon support controlled substances?\" - \"No.\"'\n  source: https://photonhealth.com/faq\nsupply_chain:\n\
  - partner: FDB Vela\n  claim: HITRUST-certified, cloud-native architecture with full redundancy and 24/7 availability for prescription transmissions.\n  source: https://photonhealth.com/faq\n  note: >-\n    HITRUST here belongs to FDB Vela, the prescription-transmission network\n    Photon routes through - NOT to Photon. Recorded as a supply-chain property\n    so it is never mistaken for a Photon certification.\nsafeguards:\n  claim: Administrative, technical, and physical safeguards for PHI.\n  source: https://photonhealth.com/faq\ngaps:\n- No SOC 2 report type (I/II), audit period, or auditor is published.\n- No subprocessor list is reachable without JavaScript.\n- No ISO 27001 or HITRUST certification is claimed by Photon itself.\ncross_references:\n  vulnerability_disclosure: none-published (see well-known/photon-well-known.yml third_party_documents)\n  domain_security: security/photon-domain-security.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/photon/refs/heads/main/security/photon-trust-center.yml
summary_line: SOC 2, HIPAA
tags:
- Healthcare
- United States
- e-Prescribing
- Pharmacy
- Prescription Routing
- GraphQL
- Clinical API
- Digital Health
- Benefit Check
- Authentication
trust_url: ''
---
