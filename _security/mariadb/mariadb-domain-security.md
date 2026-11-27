---
api_specs:
- filename: mariadb-openapi-generated.yml
  format: yaml
  label: MariaDB API
  slug: mariadb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mariadb/openapi/_ae-authored/mariadb-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mariadb.com
  spf: true
hosts:
- cert_expires: Feb 10 11:33:21 2027 GMT
  host: mariadb.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MariaDB Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MariaDB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MariaDB
provider_slug: mariadb
slug: mariadb-domain-security
source_filename: mariadb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mariadb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 11:33:21 2027 GMT\n  hsts: false\ndomains:\n- domain: mariadb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mariadb/security/mariadb-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Database
- Open Source
- Cloud
- Enterprise
- Artificial Intelligence
---
