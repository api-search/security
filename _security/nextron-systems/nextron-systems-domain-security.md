---
api_specs:
- filename: nextron-systems-info-api-openapi.yml
  format: yaml
  label: Nextron Systems Info API
  slug: nextron-systems-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextron-systems/refs/heads/main/openapi/nextron-systems-info-api-openapi.yml
- filename: nextron-systems-results-api-openapi.yml
  format: yaml
  label: Nextron Systems Results API
  slug: nextron-systems-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextron-systems/refs/heads/main/openapi/nextron-systems-results-api-openapi.yml
- filename: nextron-systems-scan-api-openapi.yml
  format: yaml
  label: Nextron Systems Scan API
  slug: nextron-systems-scan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextron-systems/refs/heads/main/openapi/nextron-systems-scan-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nextron-systems.com
  spf: true
hosts:
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: www.nextron-systems.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nextron Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nextron Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nextron Systems
provider_slug: nextron-systems
slug: nextron-systems-domain-security
source_filename: nextron-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nextron-systems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nextron-systems.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nextron-systems/refs/heads/main/security/nextron-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- Forensics
- Compromise Assessment
- Threat Detection
- Malware Analysis
- Incident Response
---
