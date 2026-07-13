---
api_specs:
- filename: kubescape-openapi.yml
  format: yaml
  label: Kubescape Posture & Compliance API
  slug: kubescape-posture-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubescape/refs/heads/main/openapi/kubescape-openapi.yml
- filename: kubescape-openapi.yml
  format: yaml
  label: Kubescape Vulnerabilities API
  slug: kubescape-vulnerabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubescape/refs/heads/main/openapi/kubescape-openapi.yml
- filename: kubescape-openapi.yml
  format: yaml
  label: Kubescape Runtime Security API
  slug: kubescape-runtime-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubescape/refs/heads/main/openapi/kubescape-openapi.yml
- filename: kubescape-openapi.yml
  format: yaml
  label: Kubescape Network Policies API
  slug: kubescape-network-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubescape/refs/heads/main/openapi/kubescape-openapi.yml
- filename: kubescape-openapi.yml
  format: yaml
  label: Kubescape Registry & Repository Scanning API
  slug: kubescape-registry-repository-scanning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubescape/refs/heads/main/openapi/kubescape-openapi.yml
- filename: kubescape-openapi.yml
  format: yaml
  label: Kubescape Access Keys API
  slug: kubescape-access-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kubescape/refs/heads/main/openapi/kubescape-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: armosec.io
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com include:_spf.google.com include:5882526.spf04.hubspotemail.net ~all
- caa: []
  dmarc: false
  dnssec: false
  domain: kubescape.io
  spf: false
hosts:
- cert_expires: Aug 21 10:40:06 2026 GMT
  host: kubescape.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 08:34:19 2026 GMT
  host: api.armosec.io
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Returns 401 without an X-API-KEY (authenticated API host).
  tls_version: TLSv1.3
- cert_expires: Aug 23 17:00:14 2026 GMT
  host: hub.armosec.io
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 10:45:31 2026 GMT
  host: cloud.armosec.io
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 07:14:19 2026 GMT
  host: armosec.io
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kubescape Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kubescape, probed live across 5 host(s) and 2 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kubescape
provider_slug: kubescape
slug: kubescape-domain-security
source_filename: kubescape-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kubescape.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 10:40:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.armosec.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 08:34:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: Returns 401 without an X-API-KEY (authenticated API host).\n- host: hub.armosec.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 17:00:14 2026 GMT\n- host: cloud.armosec.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 10:45:31 2026 GMT\n- host: armosec.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 07:14:19 2026 GMT\ndomains:\n- domain: armosec.io\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:spf.protection.outlook.com include:_spf.google.com include:5882526.spf04.hubspotemail.net\
  \ ~all\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: kubescape.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kubescape/refs/heads/main/security/kubescape-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Kubernetes Security
- Cloud Native Security
- Container Security
- DevSecOps
- Kubernetes
- Vulnerability Scanning
- Compliance
- Runtime Security
- CNCF
- Open Source
---
