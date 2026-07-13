---
api_specs:
- filename: flink-rest-api-openapi-original.yml
  format: yaml
  label: Apache Flink REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flink/refs/heads/main/openapi/flink-rest-api-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:root@apache.org"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apache.org
  spf: true
hosts:
- cert_expires: Aug 24 23:33:10 2026 GMT
  host: flink.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 08:45:06 2026 GMT
  host: nightlies.apache.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache Flink, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apache Flink
provider_slug: flink
slug: flink-domain-security
source_filename: flink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flink.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: nightlies.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 08:45:06 2026 GMT\n  hsts: false\ndomains:\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:root@apache.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flink/refs/heads/main/security/flink-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Big Data
- Distributed Computing
- Real-Time Analytics
- Stream Processing
- Workflows
---
