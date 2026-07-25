---
api_specs:
- filename: chef-channels-api-openapi.yml
  format: yaml
  label: Chef Channels API
  slug: chef-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-channels-api-openapi.yml
- filename: chef-clients-api-openapi.yml
  format: yaml
  label: Chef Clients API
  slug: chef-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-clients-api-openapi.yml
- filename: chef-cookbooks-api-openapi.yml
  format: yaml
  label: Chef Cookbooks API
  slug: chef-cookbooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-cookbooks-api-openapi.yml
- filename: chef-data-bags-api-openapi.yml
  format: yaml
  label: Chef Data Bags API
  slug: chef-data-bags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-data-bags-api-openapi.yml
- filename: chef-environments-api-openapi.yml
  format: yaml
  label: Chef Environments API
  slug: chef-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-environments-api-openapi.yml
- filename: chef-iam-api-openapi.yml
  format: yaml
  label: Chef IAM API
  slug: chef-iam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-iam-api-openapi.yml
- filename: chef-nodes-api-openapi.yml
  format: yaml
  label: Chef Nodes API
  slug: chef-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-nodes-api-openapi.yml
- filename: chef-packages-api-openapi.yml
  format: yaml
  label: Chef Packages API
  slug: chef-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-packages-api-openapi.yml
- filename: chef-profiles-api-openapi.yml
  format: yaml
  label: Chef Profiles API
  slug: chef-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-profiles-api-openapi.yml
- filename: chef-reports-api-openapi.yml
  format: yaml
  label: Chef Reports API
  slug: chef-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-reports-api-openapi.yml
- filename: chef-roles-api-openapi.yml
  format: yaml
  label: Chef Roles API
  slug: chef-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-roles-api-openapi.yml
- filename: chef-scans-api-openapi.yml
  format: yaml
  label: Chef Scans API
  slug: chef-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-scans-api-openapi.yml
- filename: chef-users-api-openapi.yml
  format: yaml
  label: Chef Users API
  slug: chef-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chef/refs/heads/main/openapi/chef-users-api-openapi.yml
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
