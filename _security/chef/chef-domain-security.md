---
api_specs:
- filename: chef-infra-server-api-openapi.yml
  format: yaml
  label: Chef Infra Server API
  slug: chef-infra-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-infra-server-api-openapi.yml
- filename: chef-automate-api-openapi.yml
  format: yaml
  label: Chef Automate API
  slug: chef-automate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-automate-api-openapi.yml
- filename: chef-habitat-builder-api-openapi.yml
  format: yaml
  label: Chef Habitat Builder API
  slug: chef-habitat-builder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-habitat-builder-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chef.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: habitat.sh
  spf: true
hosts:
- cert_expires: Sep  4 22:23:35 2026 GMT
  host: www.chef.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 22:43:43 2026 GMT
  host: docs.chef.io
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- host: docs.habitat.sh
  https: false
kind: domain-security
layout: security
method: probed
name: Chef Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chef, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Chef
provider_slug: chef
slug: chef-domain-security
source_filename: chef-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chef.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 22:23:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.chef.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 22:43:43 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.habitat.sh\n  https: false\ndomains:\n- domain: chef.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: habitat.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/security/chef-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Application Delivery
- Automation
- Compliance
- Configuration Management
- DevOps
- DevSecOps
- Habitat
- Infrastructure as Code
- InSpec
---
