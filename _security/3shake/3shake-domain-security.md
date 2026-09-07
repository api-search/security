---
api_specs:
- filename: 3shake-reckoner-external-api-openapi.yml
  format: yaml
  label: Reckoner External API
  slug: reckoner-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/3shake/refs/heads/main/openapi/3shake-reckoner-external-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 3-shake.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: reckoner-api.com
  spf: false
hosts:
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: 3-shake.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 22:43:30 2026 GMT
  host: developers.reckoner-api.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 20:41:52 2026 GMT
  host: cdp-server.reckoner-api.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: 3Shake Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 3-shake, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 3-shake
provider_slug: 3shake
slug: 3shake-domain-security
source_filename: 3shake-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 3-shake.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: false\n- host: developers.reckoner-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 22:43:30 2026 GMT\n  hsts: false\n- host: cdp-server.reckoner-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 20:41:52 2026 GMT\n  hsts: null\ndomains:\n- domain: 3-shake.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: reckoner-api.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/3shake/refs/heads/main/security/3shake-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- SRE
- Data Integration
- ETL
- iPaaS
- Workflow Automation
- Vulnerability Scanning
- Attack Surface Management
- Cloud Security
- DevSecOps
- SBOM
- Kubernetes
- Japan
---
