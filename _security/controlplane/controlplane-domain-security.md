---
api_specs:
- filename: controlplane-about-api-openapi.yml
  format: yaml
  label: ControlPlane About API
  slug: controlplane-about-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/controlplane/refs/heads/main/openapi/controlplane-about-api-openapi.yml
- filename: controlplane-artifacts-api-openapi.yml
  format: yaml
  label: ControlPlane Artifacts API
  slug: controlplane-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/controlplane/refs/heads/main/openapi/controlplane-artifacts-api-openapi.yml
- filename: controlplane-audit-api-openapi.yml
  format: yaml
  label: ControlPlane Audit API
  slug: controlplane-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/controlplane/refs/heads/main/openapi/controlplane-audit-api-openapi.yml
- filename: controlplane-controlplane-api-api-openapi.yml
  format: yaml
  label: ControlPlane ControlPlane API
  slug: controlplane-controlplane-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/controlplane/refs/heads/main/openapi/controlplane-controlplane-api-api-openapi.yml
- filename: controlplane-docker-api-openapi.yml
  format: yaml
  label: ControlPlane Docker API
  slug: controlplane-docker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/controlplane/refs/heads/main/openapi/controlplane-docker-api-openapi.yml
- filename: controlplane-health-api-openapi.yml
  format: yaml
  label: ControlPlane Health API
  slug: controlplane-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/controlplane/refs/heads/main/openapi/controlplane-health-api-openapi.yml
- filename: controlplane-helm-api-openapi.yml
  format: yaml
  label: ControlPlane Helm API
  slug: controlplane-helm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/controlplane/refs/heads/main/openapi/controlplane-helm-api-openapi.yml
- filename: controlplane-org-api-openapi.yml
  format: yaml
  label: ControlPlane Org API
  slug: controlplane-org-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/controlplane/refs/heads/main/openapi/controlplane-org-api-openapi.yml
- filename: controlplane-quota-catalog-api-openapi.yml
  format: yaml
  label: ControlPlane Quota Catalog API
  slug: controlplane-quota-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/controlplane/refs/heads/main/openapi/controlplane-quota-catalog-api-openapi.yml
- filename: controlplane-quota-increase-requests-api-openapi.yml
  format: yaml
  label: ControlPlane Quota Increase Requests API
  slug: controlplane-quota-increase-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/controlplane/refs/heads/main/openapi/controlplane-quota-increase-requests-api-openapi.yml
- filename: controlplane-resources-api-openapi.yml
  format: yaml
  label: ControlPlane Resources API
  slug: controlplane-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/controlplane/refs/heads/main/openapi/controlplane-resources-api-openapi.yml
- filename: controlplane-signups-api-openapi.yml
  format: yaml
  label: ControlPlane Signups API
  slug: controlplane-signups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/controlplane/refs/heads/main/openapi/controlplane-signups-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: controlplane.com
  spf: true
hosts:
- cert_expires: Nov 15 23:31:05 2026 GMT
  host: controlplane.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Controlplane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ControlPlane, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ControlPlane
provider_slug: controlplane
slug: controlplane-domain-security
source_filename: controlplane-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: controlplane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:31:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: controlplane.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/controlplane/refs/heads/main/security/controlplane-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cloud
- Virtualization
- Artificial Intelligence
- DevOps
---
