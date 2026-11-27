---
api_specs:
- filename: amazon-workspaces-amazon-workspaces-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Amazon WorkSpaces API
  slug: amazon-workspaces-amazon-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-workspaces/openapi/amazon-workspaces-amazon-workspaces-api-openapi.yml
- filename: amazon-workspaces-account-link-invitation-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Workspaces Account Link Invitation API
  slug: amazon-workspaces-account-link-invitation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-workspaces/openapi/amazon-workspaces-account-link-invitation-api-openapi.yml
- filename: amazon-workspaces-operations-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Workspaces Operations API
  slug: amazon-workspaces-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-workspaces/openapi/amazon-workspaces-operations-api-openapi.yml
- filename: amazon-workspaces-workspaces-pool-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Workspaces Workspaces Pool API
  slug: amazon-workspaces-workspaces-pool-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-workspaces/openapi/amazon-workspaces-workspaces-pool-api-openapi.yml
- filename: amazon-workspaces-devices-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Workspaces Devices API
  slug: amazon-workspaces-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-workspaces/openapi/amazon-workspaces-devices-api-openapi.yml
- filename: amazon-workspaces-environments-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Workspaces Environments API
  slug: amazon-workspaces-environments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-workspaces/openapi/amazon-workspaces-environments-api-openapi.yml
- filename: amazon-workspaces-softwaresets-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Workspaces Softwaresets API
  slug: amazon-workspaces-softwaresets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-workspaces/openapi/amazon-workspaces-softwaresets-api-openapi.yml
- filename: amazon-workspaces-tags-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Workspaces Tags API
  slug: amazon-workspaces-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-workspaces/openapi/amazon-workspaces-tags-api-openapi.yml
- filename: amazon-workspaces-volume-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Workspaces Volume API
  slug: amazon-workspaces-volume-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-workspaces/openapi/amazon-workspaces-volume-api-openapi.yml
- filename: amazon-workspaces-workspace-instance-api-openapi.yml
  format: yaml
  label: Amazon WorkSpaces Workspaces Workspace Instance API
  slug: amazon-workspaces-workspace-instance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-workspaces/openapi/amazon-workspaces-workspace-instance-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- host: workspaces.amazonaws.com
  https: false
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Amazon WorkSpaces Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon WorkSpaces, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon WorkSpaces
provider_slug: amazon-workspaces
slug: amazon-workspaces-domain-security
source_filename: amazon-workspaces-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: workspaces.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amazon-workspaces/security/amazon-workspaces-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Amazon Web Services
- Desktop
- End User Computing
- Virtual Desktop
- Desktop as a Service
---
