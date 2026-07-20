---
api_specs:
- filename: swagger.html
  format: yaml
  label: Cassandra REST API (Stargate)
  slug: cassandra-rest-api-stargate
  spec_type: OpenAPI
  url: https://stargate.io/docs/latest/develop/api-rest/swagger.html
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:root@apache.org"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apache.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stargate.io
  spf: true
hosts:
- cert_expires: Aug 24 23:33:10 2026 GMT
  host: cassandra.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 05:51:15 2026 GMT
  host: stargate.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cassandra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache Cassandra, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apache Cassandra
provider_slug: cassandra
slug: cassandra-domain-security
source_filename: cassandra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cassandra.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: stargate.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 05:51:15 2026 GMT\n  hsts: false\ndomains:\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:root@apache.org\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: stargate.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cassandra/refs/heads/main/security/cassandra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apache
- Big Data
- Database
- Distributed
- NoSQL
- Open Source
---
