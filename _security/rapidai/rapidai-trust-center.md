---
certifications:
- HIPAA
- GDPR
- ISO 13485
- ISO 27001
- ISO 27701
- ISO 42001
- SOC 2 Type 2
- CSA STAR
description: ''
kind: trust-center
layout: security
name: Rapidai Trust Center
name_suffix: Trust Center
overview: RapidAI maintains a public trust center documenting HIPAA, GDPR, ISO 13485, ISO 27001, ISO 27701, ISO 42001, SOC 2 Type 2, and CSA STAR compliance.
provider_name: RapidAI
provider_slug: rapidai
slug: rapidai-trust-center
source_filename: rapidai-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nprobe: true\nsource: https://www.rapidai.com/it\nurl: https://www.rapidai.com/it\nnote: RapidAI does not operate a dedicated trust portal (trust.rapidai.com, /trust,\n  /security and /compliance all miss). The published compliance posture lives on the\n  IT / infrastructure page, which names the certifications verbatim.\ncertifications:\n- HIPAA\n- GDPR\n- ISO 13485\n- ISO 27001\n- ISO 27701\n- ISO 42001\n- SOC 2 Type 2\n- CSA STAR\nframeworks:\n- NIST Cybersecurity Framework\nevidence:\n- source: https://www.rapidai.com/it\n  http_status: 200\n  quote: 'The Rapid platform has been developed using the National Institute of Standards\n    and Technology (NIST) cybersecurity framework. It is also HIPAA compliant, GDPR\n    compliant, ISO 13485, ISO 27001, ISO 27701, ISO 42001, SOC2 Type 2 and CSA Star\n    certified.'\n- source: https://www.rapidai.com/press-release/rapidai-launches-rapid-web-app-and-receives-iso-27001-certification\n\
  \  http_status: 200\n  note: Press release announcing the original ISO 27001 certification (September 2020).\n- source: https://www.rapidai.com/privacy-policy\n  http_status: 200\n  note: 'Privacy policy; EU-US Data Privacy Framework participant. Data protection\n    officer contact published: dpo@ischemaview.com'\nprobes:\n- url: https://trust.rapidai.com/\n  result: NXDOMAIN\n- url: https://www.rapidai.com/trust\n  http_status: 404\n- url: https://www.rapidai.com/security\n  http_status: 404\n- url: https://www.rapidai.com/compliance\n  http_status: 404\ngaps:\n- No public trust center / compliance portal with downloadable reports.\n- No published SOC 2 report request flow found on the public site.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rapidai/refs/heads/main/security/rapidai-trust-center.yml
summary_line: HIPAA, GDPR, ISO 13485, ISO 27001, ISO 27701, ISO 42001, SOC 2 Type 2, CSA STAR
tags:
- Healthcare
- Medical Imaging
- Artificial Intelligence
- Radiology
- Clinical Decision Support
- Stroke
- DICOM
- HL7
- FHIR
- Diagnostics
trust_url: https://www.rapidai.com/it
---
