---
certifications: []
description: ''
kind: trust-center
layout: security
name: Caresense Pte Ltd Trust Center
name_suffix: Trust Center
overview: Caresense Pte. Ltd. maintains a public trust center covering its security and compliance posture.
provider_name: Caresense Pte. Ltd.
provider_slug: caresense-pte-ltd
slug: caresense-pte-ltd-trust-center
source_filename: caresense-pte-ltd-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nprobe: true\nurl: https://trust.caresense.ai/\nplatform: Vanta Trust Center\nstatus: 200\ncertifications: []\ncertifications_note: 'The trust center is confirmed live and is a hosted Vanta Trust Center, but its\n  contents are rendered client-side by JavaScript (the served HTML is a 3.3 KB application shell) and\n  the Vanta trust-report API returns 401 without a token. No named certification (SOC 2, ISO 27001,\n  HIPAA, PDPA, GDPR) could therefore be verified during this pass, so none are recorded. Re-run with a\n  headless browser to enumerate the published frameworks and documents.'\nevidence:\n- source: https://trust.caresense.ai/\n  kind: http-probe\n  detail: HTTP 200\n- source: https://trust.caresense.ai/\n  kind: html-signature\n  detail: 'assets.vanta.com trust-report bundle; <link rel=\"canonical\" href=\"https://trust.caresense.ai\">;\n    og:title \"Trust Center\"'\n- source: https://www.caresense.ai/\n  kind: site-link\n\
  \  detail: homepage links \"Trust & Data Protection\" to https://trust.caresense.ai/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caresense-pte-ltd/refs/heads/main/security/caresense-pte-ltd-trust-center.yml
summary_line: trust center published
tags:
- Company
- Health
- Digital Health
- Artificial Intelligence
- Health Coaching
- Preventive Health
- Telemedicine
- Wellness
- Singapore
- Mobile Applications
trust_url: https://trust.caresense.ai/
---
