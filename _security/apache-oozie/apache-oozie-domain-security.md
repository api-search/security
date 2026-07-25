---
api_specs:
- filename: apache-oozie-admin-api-openapi.yml
  format: yaml
  label: Apache Oozie Admin API
  slug: apache-oozie-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-oozie/refs/heads/main/openapi/apache-oozie-admin-api-openapi.yml
- filename: apache-oozie-job-api-openapi.yml
  format: yaml
  label: Apache Oozie Job API
  slug: apache-oozie-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-oozie/refs/heads/main/openapi/apache-oozie-job-api-openapi.yml
- filename: apache-oozie-jobs-api-openapi.yml
  format: yaml
  label: Apache Oozie Jobs API
  slug: apache-oozie-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-oozie/refs/heads/main/openapi/apache-oozie-jobs-api-openapi.yml
- filename: apache-oozie-versions-api-openapi.yml
  format: yaml
  label: Apache Oozie Versions API
  slug: apache-oozie-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-oozie/refs/heads/main/openapi/apache-oozie-versions-api-openapi.yml
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
hosts:
- cert_expires: Aug 24 23:33:10 2026 GMT
  host: oozie.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apache Oozie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache Oozie, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apache Oozie
provider_slug: apache-oozie
slug: apache-oozie-domain-security
source_filename: apache-oozie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oozie.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:root@apache.org\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-oozie/refs/heads/main/security/apache-oozie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Workflow
- Hadoop
- Orchestration
- Scheduling
- Big Data
- Apache
- Java
- Open Source
---
