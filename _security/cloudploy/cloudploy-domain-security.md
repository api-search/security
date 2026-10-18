---
api_specs:
- filename: cloudploy-apps-api-openapi.yml
  format: yaml
  label: CloudPloy Apps API
  slug: cloudploy-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudploy/refs/heads/main/openapi/cloudploy-apps-api-openapi.yml
- filename: cloudploy-deployments-api-openapi.yml
  format: yaml
  label: CloudPloy Deployments API
  slug: cloudploy-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudploy/refs/heads/main/openapi/cloudploy-deployments-api-openapi.yml
- filename: cloudploy-rollback-api-openapi.yml
  format: yaml
  label: CloudPloy Rollback API
  slug: cloudploy-rollback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudploy/refs/heads/main/openapi/cloudploy-rollback-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cloudploy.com
  spf: true
hosts:
- cert_expires: Jan  6 15:59:31 2027 GMT
  host: cloudploy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cloudploy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CloudPloy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CloudPloy
provider_slug: cloudploy
slug: cloudploy-domain-security
source_filename: cloudploy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloudploy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 15:59:31 2027 GMT\n  hsts: false\ndomains:\n- domain: cloudploy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudploy/refs/heads/main/security/cloudploy-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Deployment
- Artificial Intelligence
- Cloud
- Automation
---
