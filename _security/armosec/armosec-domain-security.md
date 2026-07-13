---
api_specs:
- filename: armosec-openapi.yml
  format: yaml
  label: ARMO Vulnerabilities API
  slug: armosec-vulnerabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/openapi/armosec-openapi.yml
- filename: armosec-openapi.yml
  format: yaml
  label: ARMO Posture and Compliance API
  slug: armosec-posture-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/openapi/armosec-openapi.yml
- filename: armosec-openapi.yml
  format: yaml
  label: ARMO Clusters and Workloads API
  slug: armosec-clusters-workloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/openapi/armosec-openapi.yml
- filename: armosec-openapi.yml
  format: yaml
  label: ARMO Runtime Incidents API
  slug: armosec-runtime-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/openapi/armosec-openapi.yml
- filename: armosec-openapi.yml
  format: yaml
  label: ARMO Security Risks and Attack Chains API
  slug: armosec-security-risks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/openapi/armosec-openapi.yml
- filename: armosec-openapi.yml
  format: yaml
  label: ARMO Network and Runtime Policies API
  slug: armosec-network-runtime-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/openapi/armosec-openapi.yml
- filename: armosec-openapi.yml
  format: yaml
  label: ARMO Registry Scanning API
  slug: armosec-registry-scanning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/openapi/armosec-openapi.yml
- filename: armosec-openapi.yml
  format: yaml
  label: ARMO Integrations API
  slug: armosec-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/openapi/armosec-openapi.yml
- filename: armosec-openapi.yml
  format: yaml
  label: ARMO Access Keys API
  slug: armosec-access-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/openapi/armosec-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: armosec.io
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com include:_spf.google.com include:5882526.spf04.hubspotemail.net ~all
hosts:
- host: www.armosec.io
  hsts: false
  https: true
- host: armosec.io
  hsts: false
  https: true
- host: api.armosec.io
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
- host: hub.armosec.io
  hsts: true
  hsts_max_age: 31536000
  https: true
kind: domain-security
layout: security
method: probed
name: Armosec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ARMO, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS; 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ARMO
provider_slug: armosec
slug: armosec-domain-security
source_filename: armosec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + API hosts\nhosts:\n- host: www.armosec.io\n  https: true\n  hsts: false\n- host: armosec.io\n  https: true\n  hsts: false\n- host: api.armosec.io\n  https: true\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: hub.armosec.io\n  https: true\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: armosec.io\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:spf.protection.outlook.com include:_spf.google.com include:5882526.spf04.hubspotemail.net ~all'\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/armosec/refs/heads/main/security/armosec-domain-security.yml
summary_line: HSTS · DMARC
tags:
- Kubernetes Security
- Cloud Native Security
- CNAPP
- DevSecOps
- KSPM
- Vulnerability Management
- Compliance
- Runtime Security
- CADR
- Kubescape
- Container Security
---
