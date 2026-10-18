---
api_specs:
- filename: cloudshare-class-api-openapi.yml
  format: yaml
  label: Cloudshare Class API
  slug: cloudshare-class-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudshare/refs/heads/main/openapi/cloudshare-class-api-openapi.yml
- filename: cloudshare-classanalytics-api-openapi.yml
  format: yaml
  label: Cloudshare Class Analytics API
  slug: cloudshare-classanalytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudshare/refs/heads/main/openapi/cloudshare-classanalytics-api-openapi.yml
- filename: cloudshare-cloudfolders-api-openapi.yml
  format: yaml
  label: Cloudshare Cloudfolders API
  slug: cloudshare-cloudfolders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudshare/refs/heads/main/openapi/cloudshare-cloudfolders-api-openapi.yml
- filename: cloudshare-cloudshare-api-api-openapi.yml
  format: yaml
  label: Cloudshare Cloudshare API
  slug: cloudshare-cloudshare-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudshare/refs/heads/main/openapi/cloudshare-cloudshare-api-api-openapi.yml
- filename: cloudshare-default-api-openapi.yml
  format: yaml
  label: Cloudshare .. API
  slug: cloudshare-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudshare/refs/heads/main/openapi/cloudshare-default-api-openapi.yml
- filename: cloudshare-envs-api-openapi.yml
  format: yaml
  label: Cloudshare Envs API
  slug: cloudshare-envs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudshare/refs/heads/main/openapi/cloudshare-envs-api-openapi.yml
- filename: cloudshare-externalclouds-api-openapi.yml
  format: yaml
  label: Cloudshare Externalclouds API
  slug: cloudshare-externalclouds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudshare/refs/heads/main/openapi/cloudshare-externalclouds-api-openapi.yml
- filename: cloudshare-id-api-openapi.yml
  format: yaml
  label: Cloudshare ID API
  slug: cloudshare-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudshare/refs/heads/main/openapi/cloudshare-id-api-openapi.yml
- filename: cloudshare-instructors-api-openapi.yml
  format: yaml
  label: Cloudshare Instructors API
  slug: cloudshare-instructors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudshare/refs/heads/main/openapi/cloudshare-instructors-api-openapi.yml
- filename: cloudshare-invitations-api-openapi.yml
  format: yaml
  label: Cloudshare Invitations API
  slug: cloudshare-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudshare/refs/heads/main/openapi/cloudshare-invitations-api-openapi.yml
- filename: cloudshare-projects-api-openapi.yml
  format: yaml
  label: Cloudshare Projects API
  slug: cloudshare-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudshare/refs/heads/main/openapi/cloudshare-projects-api-openapi.yml
- filename: cloudshare-snapshots-api-openapi.yml
  format: yaml
  label: Cloudshare Snapshots API
  slug: cloudshare-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudshare/refs/heads/main/openapi/cloudshare-snapshots-api-openapi.yml
- filename: cloudshare-users-api-openapi.yml
  format: yaml
  label: Cloudshare Users API
  slug: cloudshare-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudshare/refs/heads/main/openapi/cloudshare-users-api-openapi.yml
- filename: cloudshare-vms-api-openapi.yml
  format: yaml
  label: Cloudshare Vms API
  slug: cloudshare-vms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudshare/refs/heads/main/openapi/cloudshare-vms-api-openapi.yml
- filename: cloudshare-webhooks-api-openapi.yml
  format: yaml
  label: Cloudshare Webhooks API
  slug: cloudshare-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudshare/refs/heads/main/openapi/cloudshare-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cloudshare.com
  spf: true
hosts:
- cert_expires: Dec 21 19:27:00 2026 GMT
  host: www.cloudshare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cloudshare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloudshare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cloudshare
provider_slug: cloudshare
slug: cloudshare-domain-security
source_filename: cloudshare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cloudshare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 19:27:00 2026 GMT\n  hsts: false\ndomains:\n- domain: cloudshare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudshare/refs/heads/main/security/cloudshare-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cloud
- VirtualLabs
- Training
- Sandbox
- Enterprise
---
