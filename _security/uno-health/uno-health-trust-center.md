---
certifications: []
description: ''
kind: trust-center
layout: security
name: Uno Health Trust Center
name_suffix: Trust Center
overview: Uno Health maintains a public trust center covering its security and compliance posture.
provider_name: Uno Health
provider_slug: uno-health
slug: uno-health-trust-center
source_filename: uno-health-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.unohealth.com (footer link) + DNS CNAME trust.unohealth.com -> trust.cname.drata.com\nname: Uno Health Trust Center\nurl: https://trust.unohealth.com/\nplatform: Drata\nevidence:\n- source: https://www.unohealth.com\n  detail: Homepage footer links to https://trust.unohealth.com/\n- source: dig trust.unohealth.com CNAME\n  detail: trust.cname.drata.com — Drata-hosted trust center, confirmed live (Drata SPA shell served)\ncertifications: []\nnotes: >-\n  The trust center exists and is Drata-hosted, but its content is a JS-rendered SPA\n  behind Cloudflare bot protection, so the certifications it lists could not be\n  verified by this pipeline. An earlier automated probe recorded SOC 2 / ISO 27001,\n  but those keywords came from Drata's own generic meta tags in the SPA shell, not\n  from Uno Health's published attestations — that false positive has been removed.\n  Uno Health's privacy policy (https://www.unohealth.com/legal/privacy)\
  \ references\n  HIPAA protections for member health information (compliance contact:\n  compliance@hiuno.com), consistent with a HIPAA-regulated Medicare-services company,\n  but no certification is claimed here without verification.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uno-health/refs/heads/main/security/uno-health-trust-center.yml
summary_line: trust center published
tags:
- Company
- Healthcare
- Medicare
- Benefits
- Enrollment
- Health Plans
- Government Programs
trust_url: https://trust.unohealth.com/
---
