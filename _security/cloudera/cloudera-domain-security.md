---
api_specs:
- filename: cloudera-openapi.yml
  format: yaml
  label: Cloudera CDP Public Cloud Control Plane API
  slug: cdp-control-plane
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/openapi/cloudera-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "amazonaws.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cloudera.com
  spf: true
hosts:
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: www.cloudera.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 23:59:59 2026 GMT
  host: docs.cloudera.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: api.us-west-1.cdp.cloudera.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cloudera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloudera, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cloudera
provider_slug: cloudera
slug: cloudera-domain-security
source_filename: cloudera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cloudera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: docs.cloudera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.us-west-1.cdp.cloudera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cloudera.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudera/refs/heads/main/security/cloudera-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Big Data
- Data Engineering
- Data Lakehouse
- Data Platform
- Data Warehouse
- Hadoop
- Hybrid Cloud
- Machine Learning
- Streaming
---
