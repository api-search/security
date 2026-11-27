---
api_specs:
- filename: hackerbob-ai-nlweb-api-openapi.yml
  format: yaml
  label: Hacker Bob NL Web API
  slug: hackerbob-ai-nlweb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hackerbob-ai/openapi/hackerbob-ai-nlweb-api-openapi.yml
- filename: hackerbob-ai-public-cve-records-api-openapi.yml
  format: yaml
  label: Hacker Bob Public CVE records API
  slug: hackerbob-ai-public-cve-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hackerbob-ai/openapi/hackerbob-ai-public-cve-records-api-openapi.yml
- filename: hackerbob-ai-service-api-openapi.yml
  format: yaml
  label: Hacker Bob Service API
  slug: hackerbob-ai-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hackerbob-ai/openapi/hackerbob-ai-service-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hackerbob.ai
  spf: true
hosts:
- cert_expires: Jan  1 17:28:07 2027 GMT
  host: hackerbob.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hacker Bob Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hacker Bob, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hacker Bob
provider_slug: hackerbob-ai
slug: hackerbob-ai-domain-security
source_filename: hackerbob-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hackerbob.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 17:28:07 2027 GMT\n  hsts: false\ndomains:\n- domain: hackerbob.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hackerbob-ai/security/hackerbob-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Security
- Automation
- CVE
- Offensive Security
---
