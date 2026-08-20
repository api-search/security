---
api_specs:
- filename: mithril-api-keys-api-openapi.yml
  format: yaml
  label: Mithril API Keys API
  slug: mithril-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-api-keys-api-openapi.yml
- filename: mithril-image-versions-api-openapi.yml
  format: yaml
  label: Mithril image versions API
  slug: mithril-image-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-image-versions-api-openapi.yml
- filename: mithril-instance-types-api-openapi.yml
  format: yaml
  label: Mithril instance types API
  slug: mithril-instance-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-instance-types-api-openapi.yml
- filename: mithril-instances-api-openapi.yml
  format: yaml
  label: Mithril instances API
  slug: mithril-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-instances-api-openapi.yml
- filename: mithril-kubernetes-clusters-api-openapi.yml
  format: yaml
  label: Mithril kubernetes clusters API
  slug: mithril-kubernetes-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-kubernetes-clusters-api-openapi.yml
- filename: mithril-lifecycle-scripts-api-openapi.yml
  format: yaml
  label: Mithril lifecycle scripts API
  slug: mithril-lifecycle-scripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-lifecycle-scripts-api-openapi.yml
- filename: mithril-pricing-api-openapi.yml
  format: yaml
  label: Mithril pricing API
  slug: mithril-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-pricing-api-openapi.yml
- filename: mithril-profile-api-openapi.yml
  format: yaml
  label: Mithril profile API
  slug: mithril-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-profile-api-openapi.yml
- filename: mithril-projects-api-openapi.yml
  format: yaml
  label: Mithril projects API
  slug: mithril-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-projects-api-openapi.yml
- filename: mithril-quotas-api-openapi.yml
  format: yaml
  label: Mithril quotas API
  slug: mithril-quotas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-quotas-api-openapi.yml
- filename: mithril-reservations-api-openapi.yml
  format: yaml
  label: Mithril reservations API
  slug: mithril-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-reservations-api-openapi.yml
- filename: mithril-spot-api-openapi.yml
  format: yaml
  label: Mithril spot API
  slug: mithril-spot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-spot-api-openapi.yml
- filename: mithril-ssh-keys-api-openapi.yml
  format: yaml
  label: Mithril SSH Keys API
  slug: mithril-ssh-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-ssh-keys-api-openapi.yml
- filename: mithril-volumes-api-openapi.yml
  format: yaml
  label: Mithril volumes API
  slug: mithril-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/openapi/mithril-volumes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mithril.ai
  spf: true
hosts:
- cert_expires: Aug 24 10:31:28 2026 GMT
  host: mithril.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  6 21:04:00 2026 GMT
  host: api.mithril.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mithril Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mithril, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mithril
provider_slug: mithril
slug: mithril-domain-security
source_filename: mithril-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mithril.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 10:31:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mithril.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  6 21:04:00 2026 GMT\n  hsts: null\ndomains:\n- domain: mithril.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mithril/refs/heads/main/security/mithril-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- GPU Cloud
- AI Infrastructure
- Machine-Learning
- Cloud Computing
- Compute
- Spot Instances
- Kubernetes
- GPU
---
