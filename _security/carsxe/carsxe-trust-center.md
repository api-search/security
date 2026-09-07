---
api_specs:
- filename: carsxe-specifications-api-openapi.yml
  format: yaml
  label: CarsXE Specifications API
  slug: carsxe-specifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-specifications-api-openapi.yml
- filename: carsxe-market-value-api-openapi.yml
  format: yaml
  label: CarsXE Market Value API
  slug: carsxe-market-value-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-market-value-api-openapi.yml
- filename: carsxe-plate-api-openapi.yml
  format: yaml
  label: CarsXE Plate Decoder API
  slug: carsxe-plate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-plate-api-openapi.yml
- filename: carsxe-recalls-api-openapi.yml
  format: yaml
  label: CarsXE Recalls API
  slug: carsxe-recalls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-recalls-api-openapi.yml
- filename: carsxe-history-api-openapi.yml
  format: yaml
  label: CarsXE History API
  slug: carsxe-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-history-api-openapi.yml
- filename: carsxe-images-api-openapi.yml
  format: yaml
  label: CarsXE Images API
  slug: carsxe-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-images-api-openapi.yml
- filename: carsxe-recognition-api-openapi.yml
  format: yaml
  label: CarsXE Recognition API
  slug: carsxe-recognition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-recognition-api-openapi.yml
- filename: carsxe-year-make-model-api-openapi.yml
  format: yaml
  label: CarsXE Year Make Model API
  slug: carsxe-year-make-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-year-make-model-api-openapi.yml
- filename: carsxe-lien-theft-api-openapi.yml
  format: yaml
  label: CarsXE Lien & Theft API
  slug: carsxe-lien-theft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-lien-theft-api-openapi.yml
- filename: carsxe-auth-api-openapi.yml
  format: yaml
  label: CarsXE Auth API
  slug: carsxe-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/openapi/carsxe-auth-api-openapi.yml
certification_count: 2
certifications:
- SOC 2 Type II
- ISO 27001
description: ''
kind: trust-center
layout: security
name: Carsxe Trust Center
name_suffix: Trust Center
overview: CarsXE maintains a public trust center documenting SOC 2 Type II and ISO 27001 compliance.
provider_name: CarsXE
provider_slug: carsxe
slug: carsxe-trust-center
source_filename: carsxe-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nprobe: true\nsource: https://carsxe.com/trust\nurl: https://carsxe.com/trust\nhttp_status: 200\ncertifications:\n  - name: SOC 2 Type II\n    status: certified\n    auditor: GreenHat Assurance\n    opinion: clean\n    cadence: annual\n    criteria: [Security, Availability, Confidentiality]\n    report_access: available under NDA on request via the form on the trust page\n  - name: ISO 27001\n    status: in-progress\n    note: >-\n      The page labels ISO 27001 \"In Progress\" — CarsXE states it is working toward certification, not\n      that it holds one. Recorded as in-progress so this is never read as a held certification.\ncontrols:\n  total: 75\n  domains:\n    infrastructure_security: 9\n    organizational_security: 32\n    product_security: 13\n    internal_security_procedures: 12\n    data_and_privacy: 9\nencryption:\n  at_rest: AES-256\n  in_transit: TLS 1.3\n  key_management: cloud-native KMS with automatic rotation policies\n\
  \  backups: encrypted\n  other: [certificate transparency monitoring, forward secrecy]\navailability:\n  uptime_sla: 99.9%\n  service_credits: true\n  status_page: https://carsxe.com/status\ninfrastructure:\n  provider: Google Cloud Platform\n  regions: multi-region, data primarily hosted in the United States\n  controls: [web application firewall, DDoS protection, network segmentation, RBAC, MFA, least privilege]\nvulnerability_management:\n  stated: >-\n    \"Regular penetration testing, automated vulnerability scanning, and a responsible disclosure\n    program.\"\n  disclosure_page: null\n  security_contact: null\n  note: >-\n    The trust page asserts a responsible disclosure program in prose, but CarsXE publishes no\n    disclosure page, no security.txt (404 on carsxe.com, api.carsxe.com and mcp.carsxe.com), no\n    security@ address and no bug-bounty listing. probe-security-programs.py returned vdp=none on\n    2026-09-05, so no VulnerabilityDisclosure or Security pointer is emitted\
  \ — the program is\n    claimed but not reachable, which is a real and reportable gap.\nresources:\n  - {title: \"CarsXE - Letter of Engagement from Mycroft\", format: PDF, access: request}\n  - {title: \"CarsXE SOC 2 Type 2 Report - March 2026\", format: PDF, access: request (NDA)}\nevidence:\n  - source: https://carsxe.com/trust\n    keywords: [soc 2 type ii, iso 27001, trust center, aes-256, tls 1.3, 99.9% uptime sla, responsible disclosure]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carsxe/refs/heads/main/security/carsxe-trust-center.yml
summary_line: SOC 2 Type II, ISO 27001
tags:
- Automotive
- Vehicles
- VIN
- Vehicle Data
- License Plate
- OCR
- Automobiles
- Recalls
- Market Value
- Vehicle History
- Model Context Protocol
- Agents
trust_url: https://carsxe.com/trust
---
