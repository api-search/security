---
api_specs:
- filename: coachicarus-com-agent-api-openapi.yml
  format: yaml
  label: Coach Icarus Agent API
  slug: coachicarus-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coachicarus-com/openapi/coachicarus-com-agent-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: coachicarus.com
  spf: false
hosts:
- cert_expires: Dec  8 04:09:46 2026 GMT
  host: www.coachicarus.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coach Icarus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coach Icarus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Coach Icarus
provider_slug: coachicarus-com
slug: coachicarus-com-domain-security
source_filename: coachicarus-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coachicarus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 04:09:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: coachicarus.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/coachicarus-com/security/coachicarus-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Running
- Fitness
- Coaching
- Garmin
- Health
- Wearables
- MCP
- AI Agents
---
