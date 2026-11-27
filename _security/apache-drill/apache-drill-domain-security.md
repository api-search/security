---
api_specs:
- filename: apache-drill-openapi-generated.yml
  format: yaml
  label: Apache Drill API
  slug: apache-drill-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apache-drill/openapi/_ae-authored/apache-drill-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apache.org
  spf: true
hosts:
- cert_expires: Dec 22 21:43:09 2026 GMT
  host: drill.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apache Drill Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache Drill, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Apache Drill
provider_slug: apache-drill
slug: apache-drill-domain-security
source_filename: apache-drill-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: drill.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 21:43:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/apache-drill/security/apache-drill-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SQL Engine
- Distributed Query
- Data Analytics
- Hadoop
- NoSQL
- Cloud Storage
- In‑situ Analytics
---
