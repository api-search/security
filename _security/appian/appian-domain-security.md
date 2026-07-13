---
api_specs:
- filename: appian-openapi.yml
  format: yaml
  label: Appian Application Package Details API
  slug: appian
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/openapi/appian-openapi.yml
- filename: appian-deployment-rest-openapi.yml
  format: yaml
  label: Appian Deployment REST API
  slug: deployment-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/openapi/appian-deployment-rest-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: appian.com
  spf: true
hosts:
- cert_expires: Oct 20 22:03:52 2026 GMT
  host: community.appian.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: www.appian.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: docs.appian.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Appian Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Appian, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Appian
provider_slug: appian
slug: appian-domain-security
source_filename: appian-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: community.appian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 22:03:52 2026 GMT\n  hsts: false\n- host: www.appian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.appian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: appian.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appian/refs/heads/main/security/appian-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- BPM
- Business Process Management
- Enterprise Software
- Low-Code
- Process Automation
- RPA
- Workflow
---
