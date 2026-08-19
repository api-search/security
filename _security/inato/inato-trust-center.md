---
certifications:
- ISO 27001
- HIPAA
- GDPR
description: ''
kind: trust-center
layout: security
name: Inato Trust Center
name_suffix: Trust Center
overview: Inato maintains a public trust center documenting ISO 27001, HIPAA, and GDPR compliance.
provider_name: Inato
provider_slug: inato
slug: inato-trust-center
source_filename: inato-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nprobe: true\nsource: https://support.inato.com/data-security\nurl: https://support.inato.com/data-security\ntrust_center:\n  platform: Drata\n  url: https://app.drata.com/trust/9cb59bcb-0c38-11ee-865f-029d78a187d9\n  discovered_in: >-\n    the \"Contact Our Security Team\" block of support.inato.com/data-security\n    (extracted from the site's client-side bundle, since the page is\n    JS-rendered)\n  readable: false\n  probe:\n    status: 403\n    detail: >-\n      Cloudflare bot challenge (\"Just a moment...\") on app.drata.com; the Drata\n      public API (public-api.drata.com/public/trust-center/<id>) answers 401\n      Unauthorized. The trust center is real and Inato-owned, but its contents —\n      including whatever audit reports Drata is tracking — could not be read by\n      machine on 2026-08-17. Certifications below are therefore taken from\n      Inato's own security page, not from the trust center.\ncertifications:\n\
  - ISO 27001\n- HIPAA\n- GDPR\ncertifications_not_claimed:\n- SOC 2\n- 21 CFR Part 11\n- HITRUST\n- PCI DSS\n- FedRAMP\nframeworks:\n- name: HIPAA\n  detail: 'HIPAA \"Preparatory to Research\" (45 CFR 164.512); Business Associate Agreement (BAA) available and required before any EHR connector is enabled'\n- name: ISO 27001\n  detail: Information security management — claimed as a badge; certificate available on request, not published\n- name: GDPR\n  detail: >-\n    EU data protection. Inato states the processor posture explicitly: \"Inato\n    processes the data on your behalf, under your instruction and\n    authorization.\" Regional data-residency commitments claimed for the GCP\n    environment.\ncontrols:\n- encryption: AES-256 for data at rest and in transit\n- de_identification: >-\n    Names, dates of birth, addresses and contact details are stripped the moment\n    a file is uploaded or synced, before any AI processing begins\n- pseudonymization: Records pseudonymized and stored\
  \ under random identifiers in secure Google Cloud storage\n- data_hosting: Google Cloud Platform (Inato-owned projects)\n- network_defense: Google Cloud Armor for DDoS and external threat defense\n- access_control: >-\n    Logical access controls designed to prevent Inato staff from viewing\n    identifiable patient data; sponsors see only aggregated, de-identified\n    pre-screening insights\n- retention: Original uploaded files are not retained in viewable form\n- integration_posture: >-\n    EHR integrations are read-only bulk FHIR — architecturally unable to write,\n    modify or delete data in the site's EHR, and the site approves the access\n    scope inside its own EHR\nai_governance:\n- model: Google Gemini, deployed inside Inato's own Google Cloud projects\n- no_third_party_llm: Patient data is never sent to any third-party US-based LLM provider\n- no_training: >-\n    No site or patient data is used to train AI models; Google does not use it to\n    train their foundation models.\
  \ Non-patient signals (user feedback on AI\n    response accuracy) may be used to tune prompts and configuration\n- human_in_the_loop: >-\n    The AI flags and summarizes; the site team reviews every patient and makes\n    every final call before anyone moves to screening\n- explainability: >-\n    Criterion-by-criterion summary of met / not met / unknown with the clinical\n    evidence relied on, which the site team can read, challenge and override\n- bias_control: Each patient is assessed against protocol criteria individually, never ranked against other patients\n- purpose_limitation: >-\n    Patient data is processed solely for the site's specific trial — not for\n    product development, AI training or research, except as agreed in writing\ncontact: security@inato.com\ndocumentation_on_request: >-\n  Compliance documentation, security-review templates and the BAA are offered via\n  security@inato.com rather than published for download.\nevidence:\n- source: https://support.inato.com/data-security\n\
  \  keywords: [iso 27001, hipaa, gdpr, aes-256, business associate agreement, google gemini, cloud armor, de-identification]\n- source: https://app.drata.com/trust/9cb59bcb-0c38-11ee-865f-029d78a187d9\n  status: 403\n  keywords: [drata, trust center]\nweakest_link:\n  connector: AdvancedMD\n  detail: >-\n    The AdvancedMD connector is credential-based: the site shares its AdvancedMD\n    login name, password and Office Key with Inato. Inato's own guidance\n    recommends creating a dedicated AdvancedMD account for Inato. This is the one\n    connector that is not token- or FHIR-scoped, and it sits inside an otherwise\n    strong read-only posture.\n  source: https://support.inato.com/connections/advancedmd\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inato/refs/heads/main/security/inato-trust-center.yml
summary_line: ISO 27001, HIPAA, GDPR
tags:
- Company
- Clinical Trials
- Healthcare
- Life Sciences
- Pharmaceuticals
- Clinical Research
- Marketplace
- Artificial Intelligence
trust_url: https://support.inato.com/data-security
---
