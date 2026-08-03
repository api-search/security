---
certifications: []
description: ''
kind: trust-center
layout: security
name: Noom Trust Center
name_suffix: Trust Center
overview: Noom maintains a public trust center covering its security and compliance posture.
provider_name: Noom
provider_slug: noom
slug: noom-trust-center
source_filename: noom-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nprobe: true\nurl: https://trust.noom.com/\ntitle: Noom, Inc. Trust Center\nplatform: Vanta\nplatform_evidence:\n  asset_host: assets.vanta.com\n  trust_report_bundle: https://assets.vanta.com/static/index-trust-report.a8f7a62c.js\n  slug_id: dgdmws2fcocud955j00d2l\n  document_proxy: https://app.vanta.com/doc?s=az7pnjh8rqk4qy1cpruk\ncertifications: []\ncertifications_note: >-\n  The trust center is confirmed live (HTTP 200, canonical https://trust.noom.com,\n  page title \"Noom, Inc. Trust Center\", served by Vanta), but the control, framework\n  and certification list is rendered client-side by the Vanta trust-report bundle and\n  is not present in the anonymous HTML response. No certification (SOC 2, ISO 27001,\n  HITRUST, PCI DSS, FedRAMP) could be verified anonymously, and none is asserted here.\n  Vanta trust centers commonly gate document access behind an NDA/access request.\n  Re-probe with a rendering client to populate this list.\n\
  related_compliance_disclosures:\n- kind: HIPAA Notice of Privacy Practices\n  url: https://www.noom.com/hipaa-notice/\n  http_status: 200\n- kind: Privacy Policy\n  url: https://www.noom.com/noom-privacy-policy/\n  http_status: 200\n- kind: Consumer Health Data Privacy Notice\n  url: https://www.noom.com/consumer-health-data-privacy-notice/\n  http_status: 200\n- kind: Cookie Policy\n  url: https://www.noom.com/cookie-policy/\n  http_status: 200\nevidence:\n- source: https://trust.noom.com/\n  http_status: 200\n  content_type: text/html\n  signals:\n  - '<title>Noom, Inc. Trust Center</title>'\n  - '<link rel=\"canonical\" href=\"https://trust.noom.com\">'\n  - vanta trust-report stylesheet + script bundle\nx-evidence:\n  fetched: '2026-07-31'\n  url: https://trust.noom.com/\n  http_status: 200\n  content_type: text/html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noom/refs/heads/main/security/noom-trust-center.yml
summary_line: trust center published
tags:
- Company
- Health
- Digital Health
- Weight Management
- Wellness
- Behavioral Health
- Telehealth
- Nutrition
- Consumer Health
- Mobile Applications
trust_url: https://trust.noom.com/
---
