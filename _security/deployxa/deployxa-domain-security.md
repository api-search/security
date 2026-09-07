---
api_specs:
- filename: deployxa-openapi-original.json
  format: json
  label: Deployxa Platform
  slug: deployxa-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deployxa/refs/heads/main/openapi/deployxa-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: deployxa.com
  spf: true
hosts:
- cert_expires: Oct 25 11:16:27 2026 GMT
  host: deployxa.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Deployxa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deployxa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Deployxa
provider_slug: deployxa
slug: deployxa-domain-security
source_filename: deployxa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deployxa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 11:16:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: deployxa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deployxa/refs/heads/main/security/deployxa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- platform-as-a-service
- cloud-deployment
- devops
- ci-cd
- containers-docker
- edge-hosting
- managed-databases
- ai-ops
- developer-tools
---
