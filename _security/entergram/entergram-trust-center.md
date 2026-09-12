---
api_specs:
- filename: entergram-openapi.json
  format: json
  label: Entergram API
  slug: entergram-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/openapi/entergram-openapi.json
certification_count: 0
certifications: []
description: ''
kind: trust-center
layout: security
name: Entergram Trust Center
name_suffix: Trust Center
overview: Entergram maintains a public trust center covering its security and compliance posture.
provider_name: Entergram
provider_slug: entergram
slug: entergram-trust-center
source_filename: entergram-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-11'\nmethod: searched\nsource: https://www.entergram.com/security\ntrust_page: https://www.entergram.com/security\ncertifications: []\ncompliance_programs:\n- name: GDPR\n  status: aligned\n  note: Self-attested alignment stated on the security page; no third-party certificate published.\ncontrols:\n- Encryption at rest with AES-256-GCM (Telegram session custody)\n- TLS encryption in transit (HTTPS everywhere)\n- Dedicated proxy IP per connected Telegram account\n- Least-privilege, scoped and audited access to decryption\n- Workspace isolation (a key from workspace A cannot access workspace B)\n- Configurable API-key/OAuth TTL, optional IP allowlists, instant revocation, audit logging\nnote: >-\n  No SOC 2, ISO 27001, PCI or HIPAA certification is claimed. The security posture is described in\n  prose on the security page rather than in a formal trust portal with downloadable reports.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/entergram/refs/heads/main/security/entergram-trust-center.yml
summary_line: trust center published
tags:
- Messaging
- Notifications
- Communications
- CRM
- Telegram
- Customer Support
- Ticketing
- Sales
- MCP
- Webhooks
trust_url: ''
---
