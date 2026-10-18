---
api_specs:
- filename: connectly-businesses-api-openapi.yml
  format: yaml
  label: Connectly Businesses API
  slug: connectly-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connectly/refs/heads/main/openapi/connectly-businesses-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: connectly.ai
  spf: true
hosts:
- cert_expires: Nov 17 23:00:09 2026 GMT
  host: www.connectly.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Connectly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Connectly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Connectly
provider_slug: connectly
slug: connectly-domain-security
source_filename: connectly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.connectly.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:00:09 2026 GMT\n  hsts: false\ndomains:\n- domain: connectly.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connectly/refs/heads/main/security/connectly-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Platform
- CustomerEngagement
- Enterprise
- Automation
---
