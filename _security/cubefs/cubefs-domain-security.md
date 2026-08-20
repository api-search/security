---
api_specs:
- filename: cubefs-acls-api-openapi.yml
  format: yaml
  label: CubeFS ACLs API
  slug: cubefs-acls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/openapi/cubefs-acls-api-openapi.yml
- filename: cubefs-buckets-api-openapi.yml
  format: yaml
  label: CubeFS Buckets API
  slug: cubefs-buckets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/openapi/cubefs-buckets-api-openapi.yml
- filename: cubefs-cluster-api-openapi.yml
  format: yaml
  label: CubeFS Cluster API
  slug: cubefs-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/openapi/cubefs-cluster-api-openapi.yml
- filename: cubefs-datanodes-api-openapi.yml
  format: yaml
  label: CubeFS DataNodes API
  slug: cubefs-datanodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/openapi/cubefs-datanodes-api-openapi.yml
- filename: cubefs-datapartitions-api-openapi.yml
  format: yaml
  label: CubeFS DataPartitions API
  slug: cubefs-datapartitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/openapi/cubefs-datapartitions-api-openapi.yml
- filename: cubefs-metanodes-api-openapi.yml
  format: yaml
  label: CubeFS MetaNodes API
  slug: cubefs-metanodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/openapi/cubefs-metanodes-api-openapi.yml
- filename: cubefs-metapartitions-api-openapi.yml
  format: yaml
  label: CubeFS MetaPartitions API
  slug: cubefs-metapartitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/openapi/cubefs-metapartitions-api-openapi.yml
- filename: cubefs-multipart-api-openapi.yml
  format: yaml
  label: CubeFS Multipart API
  slug: cubefs-multipart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/openapi/cubefs-multipart-api-openapi.yml
- filename: cubefs-objects-api-openapi.yml
  format: yaml
  label: CubeFS Objects API
  slug: cubefs-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/openapi/cubefs-objects-api-openapi.yml
- filename: cubefs-users-api-openapi.yml
  format: yaml
  label: CubeFS Users API
  slug: cubefs-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/openapi/cubefs-users-api-openapi.yml
- filename: cubefs-volumes-api-openapi.yml
  format: yaml
  label: CubeFS Volumes API
  slug: cubefs-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/openapi/cubefs-volumes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cubefs.io
  spf: false
hosts:
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: cubefs.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cubefs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CubeFS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: CubeFS
provider_slug: cubefs
slug: cubefs-domain-security
source_filename: cubefs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cubefs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: cubefs.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cubefs/refs/heads/main/security/cubefs-domain-security.yml
summary_line: TLSv1.3
tags:
- Cloud-Native
- CNCF Graduated
- Distributed File System
- Kubernetes
- Object Storage
- POSIX
- S3 Compatible
- Storage
---
