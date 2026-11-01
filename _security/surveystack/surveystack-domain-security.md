---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: surveystack.io
  spf: true
hosts:
- host: surveystack.io
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Surveystack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SurveyStack, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SurveyStack
provider_slug: surveystack
slug: surveystack-domain-security
source_filename: surveystack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: surveystack.io\n  https: false\ndomains:\n- domain: surveystack.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/surveystack/security/surveystack-domain-security.yml
summary_line: DMARC
tags:
- SurveyStack
- Data Collection
- Analytics
- Community
- API
---
