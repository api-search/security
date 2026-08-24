---
api_specs:
- filename: kontaktio-device-management-openapi.yml
  format: yaml
  label: Kontakt.io Device Management API
  slug: kontaktio-device-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontaktio/refs/heads/main/openapi/kontaktio-device-management-openapi.yml
- filename: kontaktio-location-occupancy-openapi.yml
  format: yaml
  label: Kontakt.io Location & Occupancy API
  slug: kontaktio-location-occupancy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontaktio/refs/heads/main/openapi/kontaktio-location-occupancy-openapi.yml
- filename: kontaktio-spaces-openapi.yml
  format: yaml
  label: Kontakt.io Spaces API
  slug: kontaktio-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontaktio/refs/heads/main/openapi/kontaktio-spaces-openapi.yml
- filename: kontaktio-entity-management-openapi.yml
  format: yaml
  label: Kontakt.io Entity Management Integration API
  slug: kontaktio-entity-management-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontaktio/refs/heads/main/openapi/kontaktio-entity-management-openapi.yml
certifications:
- SOC 2 Type II
- HIPAA Security Rule / HITECH
- GDPR
- ISO 27001
description: ''
kind: trust-center
layout: security
name: Kontaktio Trust Center
name_suffix: Trust Center
overview: Kontakt.io maintains a public trust center documenting SOC 2 Type II, HIPAA Security Rule / HITECH, GDPR, and ISO 27001 compliance.
provider_name: Kontakt.io
provider_slug: kontaktio
slug: kontaktio-trust-center
source_filename: kontaktio-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: searched\nsource: https://trust.kontakt.io/ and https://kontakt.io/legal-documents/security/\ntrust_center:\n  url: https://trust.kontakt.io/\n  platform: Vanta\n  http_status: 200\n  probed: '2026-08-23'\n  note: Canonical Vanta-hosted trust center (canonical link rel points at https://trust.kontakt.io;\n    assets served from assets.vanta.com). Document access is request-gated behind Vanta,\n    which is normal for this platform — the certification claims below are read from\n    Kontakt.io's own public security page, not from gated Vanta artifacts.\nsecurity_page: https://kontakt.io/legal-documents/security/\nsecurity_officer: Lemlem Kentiba, Security & Compliance Officer\ncertifications:\n- name: SOC 2 Type II\n  status: compliant\n  source: https://kontakt.io/legal-documents/security/\n- name: HIPAA Security Rule / HITECH\n  status: compliant\n  source: https://kontakt.io/legal-documents/security/\n- name: GDPR\n  status: aligned\n  source:\
  \ https://kontakt.io/legal-documents/security/\n- name: ISO 27001\n  status: not-claimed\n  source: Absent from the security page and the trust center landing page.\ncontrols:\n  encryption_in_transit: TLS 1.2+ across all external and internal communications.\n  encryption_at_rest: AWS S3 encryption, encrypted EBS volumes, encrypted RDS/Aurora\n    databases and encrypted backups.\n  key_management: AWS KMS with FIPS 140-2 validated hardware security modules; key\n    access is role-restricted and monitored.\n  penetration_testing: External penetration tests conducted regularly by independent\n    third parties; findings undergo formal tracking and remediation.\nvulnerability_disclosure:\n  program: false\n  note: 'No vulnerability disclosure program, bug bounty, or responsible-disclosure\n    contact was found. There is no /.well-known/security.txt on any Kontakt.io host,\n    no HackerOne/Bugcrowd/Intigriti presence, and the public security page names a\n    Security & Compliance Officer\
  \ but publishes no security contact address. The only\n    reporting route is general support at https://support.kontakt.io/hc/en-gb/requests/new.\n    This is the single clearest security-posture gap for a vendor holding SOC 2 Type\n    II and HIPAA. No Security / VulnerabilityDisclosure pointer is emitted.'\n  evidence:\n  - url: https://kontakt.io/.well-known/security.txt\n    status: 404\n  - url: https://developer.kontakt.io/.well-known/security.txt\n    status: 404\n  - url: https://kontakt.io/legal-documents/security/\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kontaktio/refs/heads/main/security/kontaktio-trust-center.yml
summary_line: SOC 2 Type II, HIPAA Security Rule / HITECH, GDPR, ISO 27001
tags:
- Company
- IoT
- RTLS
- Healthcare
- Asset Tracking
- Location
- Occupancy
- Bluetooth
- Device Management
- Telemetry
- Sensors
- Streaming
trust_url: ''
---
