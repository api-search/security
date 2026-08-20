---
api_specs:
- filename: nutanix-alerts-api-openapi.yml
  format: yaml
  label: Nutanix Alerts API
  slug: nutanix-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-alerts-api-openapi.yml
- filename: nutanix-categories-api-openapi.yml
  format: yaml
  label: Nutanix Categories API
  slug: nutanix-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-categories-api-openapi.yml
- filename: nutanix-clusters-api-openapi.yml
  format: yaml
  label: Nutanix Clusters API
  slug: nutanix-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-clusters-api-openapi.yml
- filename: nutanix-hosts-api-openapi.yml
  format: yaml
  label: Nutanix Hosts API
  slug: nutanix-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-hosts-api-openapi.yml
- filename: nutanix-images-api-openapi.yml
  format: yaml
  label: Nutanix Images API
  slug: nutanix-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-images-api-openapi.yml
- filename: nutanix-network-security-rules-api-openapi.yml
  format: yaml
  label: Nutanix Network Security Rules API
  slug: nutanix-network-security-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-network-security-rules-api-openapi.yml
- filename: nutanix-projects-api-openapi.yml
  format: yaml
  label: Nutanix Projects API
  slug: nutanix-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-projects-api-openapi.yml
- filename: nutanix-protection-domains-api-openapi.yml
  format: yaml
  label: Nutanix Protection Domains API
  slug: nutanix-protection-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-protection-domains-api-openapi.yml
- filename: nutanix-snapshots-api-openapi.yml
  format: yaml
  label: Nutanix Snapshots API
  slug: nutanix-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-snapshots-api-openapi.yml
- filename: nutanix-storage-containers-api-openapi.yml
  format: yaml
  label: Nutanix Storage Containers API
  slug: nutanix-storage-containers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-storage-containers-api-openapi.yml
- filename: nutanix-storage-pools-api-openapi.yml
  format: yaml
  label: Nutanix Storage Pools API
  slug: nutanix-storage-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-storage-pools-api-openapi.yml
- filename: nutanix-subnets-api-openapi.yml
  format: yaml
  label: Nutanix Subnets API
  slug: nutanix-subnets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-subnets-api-openapi.yml
- filename: nutanix-virtual-disks-api-openapi.yml
  format: yaml
  label: Nutanix Virtual Disks API
  slug: nutanix-virtual-disks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-virtual-disks-api-openapi.yml
- filename: nutanix-vms-api-openapi.yml
  format: yaml
  label: Nutanix VMs API
  slug: nutanix-vms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-vms-api-openapi.yml
- filename: nutanix-webhooks-api-openapi.yml
  format: yaml
  label: Nutanix Webhooks API
  slug: nutanix-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@nutanix.com"
  - 0 issue "amazon.com"
  - 0 issue "certainly.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nutanix.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: nutanix.dev
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: www.nutanix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: www.nutanix.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.nutanix.com
  https: false
kind: domain-security
layout: security
method: probed
name: Nutanix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nutanix, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nutanix
provider_slug: nutanix
slug: nutanix-domain-security
source_filename: nutanix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nutanix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.nutanix.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.nutanix.com\n  https: false\ndomains:\n- domain: nutanix.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:security@nutanix.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: nutanix.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/security/nutanix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Management
- Hyper-Converged
- Infrastructure
- Virtualization
- Kubernetes
- Database
---
