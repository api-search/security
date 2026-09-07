---
api_specs:
- filename: dentsply-sirona-intraoral-modality-openapi.yml
  format: yaml
  label: Dentsply Sirona Intraoral Imaging Modality API
  slug: dsio-modality-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dentsply-sirona/refs/heads/main/openapi/dentsply-sirona-intraoral-modality-openapi.yml
- filename: dentsply-sirona-intraoral-filters-openapi.yml
  format: yaml
  label: Dentsply Sirona Intraoral Imaging Filters API
  slug: dsio-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dentsply-sirona/refs/heads/main/openapi/dentsply-sirona-intraoral-filters-openapi.yml
- filename: dentsply-sirona-intraoral-exposure-openapi.yml
  format: yaml
  label: Intraoral Exposure API
  slug: io-exposure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dentsply-sirona/refs/heads/main/openapi/dentsply-sirona-intraoral-exposure-openapi.yml
certification_count: 0
certifications: []
description: ''
kind: trust-center
layout: security
name: Dentsply Sirona Trust Center
name_suffix: Trust Center
overview: Dentsply Sirona maintains a public trust center covering its security and compliance posture.
provider_name: Dentsply Sirona
provider_slug: dentsply-sirona
slug: dentsply-sirona-trust-center
source_filename: dentsply-sirona-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nprobe: true\nfound: false\nnotes: >-\n  No trust center was found. trust.dentsplysirona.com and security.dentsplysirona.com do not\n  resolve. The site footer links a \"Trust Center\" at\n  https://coresupport.dentsplysirona.com/doc/cm-trust-center-en-US/- which returns HTTP 200 but is\n  a 13.6 KB JavaScript application shell whose only rendered text is \"Support\" — no certifications,\n  no compliance statements, no security posture, nothing a machine or a person can read without an\n  authenticated session. Dentsply Sirona does publish medical-device and ESG compliance material\n  (ISO 13485, MDR, FDA), but no SOC 2 / ISO 27001 / HIPAA / PCI attestation for its cloud or API\n  surface is publicly reachable, so no Compliance pointer is claimed.\ncertifications: []\nevidence:\n- source: https://coresupport.dentsplysirona.com/doc/cm-trust-center-en-US/-\n  http_status: 200\n  bytes: 13627\n  note: JS shell; rendered body is the single\
  \ word \"Support\"\n- source: https://trust.dentsplysirona.com/\n  http_status: 000\n  note: does not resolve\n- source: https://security.dentsplysirona.com/\n  http_status: 000\n  note: does not resolve\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dentsply-sirona/refs/heads/main/security/dentsply-sirona-trust-center.yml
summary_line: trust center published
tags:
- CAD/CAM
- CEREC
- Dental
- DS Core
- Imaging
- Intraoral Imaging
- Lab Management
- Medical Devices
- Practice Management
- Fortune 1000
trust_url: ''
---
