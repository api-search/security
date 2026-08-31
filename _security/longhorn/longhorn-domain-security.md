---
api_specs:
- filename: longhorn-backingimages-api-openapi.yml
  format: yaml
  label: Longhorn BackingImages API
  slug: longhorn-backingimages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/longhorn/refs/heads/main/openapi/longhorn-backingimages-api-openapi.yml
- filename: longhorn-backups-api-openapi.yml
  format: yaml
  label: Longhorn Backups API
  slug: longhorn-backups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/longhorn/refs/heads/main/openapi/longhorn-backups-api-openapi.yml
- filename: longhorn-engineimages-api-openapi.yml
  format: yaml
  label: Longhorn EngineImages API
  slug: longhorn-engineimages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/longhorn/refs/heads/main/openapi/longhorn-engineimages-api-openapi.yml
- filename: longhorn-nodes-api-openapi.yml
  format: yaml
  label: Longhorn Nodes API
  slug: longhorn-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/longhorn/refs/heads/main/openapi/longhorn-nodes-api-openapi.yml
- filename: longhorn-recurringjobs-api-openapi.yml
  format: yaml
  label: Longhorn RecurringJobs API
  slug: longhorn-recurringjobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/longhorn/refs/heads/main/openapi/longhorn-recurringjobs-api-openapi.yml
- filename: longhorn-settings-api-openapi.yml
  format: yaml
  label: Longhorn Settings API
  slug: longhorn-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/longhorn/refs/heads/main/openapi/longhorn-settings-api-openapi.yml
- filename: longhorn-snapshots-api-openapi.yml
  format: yaml
  label: Longhorn Snapshots API
  slug: longhorn-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/longhorn/refs/heads/main/openapi/longhorn-snapshots-api-openapi.yml
- filename: longhorn-systembackups-api-openapi.yml
  format: yaml
  label: Longhorn SystemBackups API
  slug: longhorn-systembackups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/longhorn/refs/heads/main/openapi/longhorn-systembackups-api-openapi.yml
- filename: longhorn-volumes-api-openapi.yml
  format: yaml
  label: Longhorn Volumes API
  slug: longhorn-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/longhorn/refs/heads/main/openapi/longhorn-volumes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: longhorn.io
  spf: true
hosts:
- cert_expires: Aug 27 16:21:04 2026 GMT
  host: longhorn.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Longhorn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Longhorn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Longhorn
provider_slug: longhorn
slug: longhorn-domain-security
source_filename: longhorn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: longhorn.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 16:21:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: longhorn.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/longhorn/refs/heads/main/security/longhorn-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Backup
- Block Storage
- Cloud-Native
- Incubating
- Kubernetes
- Persistent Volumes
---
