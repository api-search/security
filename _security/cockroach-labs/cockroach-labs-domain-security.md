---
api_specs:
- filename: cockroach-labs-cloud-api-openapi.yml
  format: yaml
  label: CockroachDB Cloud API
  slug: cockroach-labs-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cockroach-labs/refs/heads/main/openapi/cockroach-labs-cloud-api-openapi.yml
- filename: cockroach-labs-cluster-api-openapi.yml
  format: yaml
  label: CockroachDB Cluster API
  slug: cockroach-labs-cluster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cockroach-labs/refs/heads/main/openapi/cockroach-labs-cluster-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cockroachlabs.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cockroachlabs.cloud
  spf: true
hosts:
- cert_expires: Aug 30 23:24:02 2026 GMT
  host: www.cockroachlabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 09:40:24 2026 GMT
  host: cockroachlabs.cloud
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cockroach Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cockroach Labs, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cockroach Labs
provider_slug: cockroach-labs
slug: cockroach-labs-domain-security
source_filename: cockroach-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cockroachlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 23:24:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cockroachlabs.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 09:40:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cockroachlabs.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cockroachlabs.cloud\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cockroach-labs/refs/heads/main/security/cockroach-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cluster Management
- Cloud
- Database
- Distributed SQL
- Infrastructure
- PostgreSQL Compatible
- SQL
---
