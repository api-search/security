---
api_specs:
- filename: yugabyte-backup-info-api-openapi.yml
  format: yaml
  label: Yugabyte backup-info API
  slug: yugabyte-backup-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yugabyte/refs/heads/main/openapi/yugabyte-backup-info-api-openapi.yml
- filename: yugabyte-cluster-api-openapi.yml
  format: yaml
  label: Yugabyte cluster API
  slug: yugabyte-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yugabyte/refs/heads/main/openapi/yugabyte-cluster-api-openapi.yml
- filename: yugabyte-cluster-info-api-openapi.yml
  format: yaml
  label: Yugabyte cluster-info API
  slug: yugabyte-cluster-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yugabyte/refs/heads/main/openapi/yugabyte-cluster-info-api-openapi.yml
- filename: yugabyte-pitr-info-api-openapi.yml
  format: yaml
  label: Yugabyte pitr-info API
  slug: yugabyte-pitr-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yugabyte/refs/heads/main/openapi/yugabyte-pitr-info-api-openapi.yml
- filename: yugabyte-restore-info-api-openapi.yml
  format: yaml
  label: Yugabyte restore-info API
  slug: yugabyte-restore-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yugabyte/refs/heads/main/openapi/yugabyte-restore-info-api-openapi.yml
- filename: yugabyte-voyager-info-api-openapi.yml
  format: yaml
  label: Yugabyte voyager-info API
  slug: yugabyte-voyager-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yugabyte/refs/heads/main/openapi/yugabyte-voyager-info-api-openapi.yml
- filename: yugabyte-voyager-metrics-api-openapi.yml
  format: yaml
  label: Yugabyte voyager-metrics API
  slug: yugabyte-voyager-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yugabyte/refs/heads/main/openapi/yugabyte-voyager-metrics-api-openapi.yml
- filename: yugabyte-xcluster-metrics-api-openapi.yml
  format: yaml
  label: Yugabyte Xcluster Metrics API
  slug: yugabyte-xcluster-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yugabyte/refs/heads/main/openapi/yugabyte-xcluster-metrics-api-openapi.yml
- filename: yugabyte-xcluster-namespace-details-api-openapi.yml
  format: yaml
  label: Yugabyte Xcluster Namespace Details API
  slug: yugabyte-xcluster-namespace-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yugabyte/refs/heads/main/openapi/yugabyte-xcluster-namespace-details-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: yugabyte.com
  spf: true
hosts:
- cert_expires: Sep 16 06:25:05 2026 GMT
  host: api-docs.yugabyte.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 20:27:57 2026 GMT
  host: cloud.yugabyte.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 07:23:46 2026 GMT
  host: docs.yugabyte.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yugabyte Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yugabyte, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Yugabyte
provider_slug: yugabyte
slug: yugabyte-domain-security
source_filename: yugabyte-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api-docs.yugabyte.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 06:25:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud.yugabyte.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 20:27:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.yugabyte.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 07:23:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: yugabyte.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yugabyte/refs/heads/main/security/yugabyte-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Database
- Distributed SQL
- PostgreSQL
- Cloud
- Database-as-a-Service
- Open-Source
- SQL
- Data
- Infrastructure
---
