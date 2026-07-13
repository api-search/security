---
api_specs:
- filename: bettercloud-platform-api.yaml
  format: yaml
  label: BetterCloud Platform API
  slug: bettercloud-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/openapi/bettercloud-platform-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bettercloud.com
  spf: true
hosts:
- cert_expires: Aug 25 01:01:31 2026 GMT
  host: developer.bettercloud.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 07:26:07 2026 GMT
  host: api.bettercloud.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bettercloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BetterCloud, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: BetterCloud
provider_slug: bettercloud
slug: bettercloud-domain-security
source_filename: bettercloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.bettercloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 01:01:31 2026 GMT\n  hsts: false\n- host: api.bettercloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 07:26:07 2026 GMT\n  hsts: null\ndomains:\n- domain: bettercloud.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bettercloud/refs/heads/main/security/bettercloud-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Automation
- Compliance
- Enterprise
- IT Operations
- SaaS Management
- Security
- Workflows
- User Lifecycle
---
