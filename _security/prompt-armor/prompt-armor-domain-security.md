---
api_specs:
- filename: prompt-armor-openapi.yml
  format: yaml
  label: PromptArmor Content Check API
  slug: prompt-armor-content-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prompt-armor/refs/heads/main/openapi/prompt-armor-openapi.yml
- filename: prompt-armor-openapi.yml
  format: yaml
  label: PromptArmor Analyze API
  slug: prompt-armor-analyze-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prompt-armor/refs/heads/main/openapi/prompt-armor-openapi.yml
- filename: prompt-armor-openapi.yml
  format: yaml
  label: PromptArmor Session Monitoring API
  slug: prompt-armor-session-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prompt-armor/refs/heads/main/openapi/prompt-armor-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: promptarmor.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Sep 19 19:15:36 2026 GMT
  host: www.promptarmor.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: promptarmor.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 19:59:36 2026 GMT
  host: api.promptarmor.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prompt Armor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PromptArmor, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PromptArmor
provider_slug: prompt-armor
slug: prompt-armor-domain-security
source_filename: prompt-armor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.promptarmor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 19:15:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: promptarmor.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.promptarmor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 19:59:36 2026 GMT\n  hsts: null\ndomains:\n- domain: promptarmor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prompt-armor/refs/heads/main/security/prompt-armor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LLM
- Security
- Prompt Injection
- Threat Detection
---
