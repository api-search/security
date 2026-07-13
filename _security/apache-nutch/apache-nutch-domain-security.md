---
api_specs:
- filename: apache-nutch-openapi.yaml
  format: yaml
  label: Apache Nutch REST API
  slug: apache-nutch-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/openapi/apache-nutch-openapi.yaml
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
- cert_expires: Sep 10 04:10:25 2026 GMT
  host: cwiki.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apache Nutch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache Nutch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apache Nutch
provider_slug: apache-nutch
slug: apache-nutch-domain-security
source_filename: apache-nutch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cwiki.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 04:10:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:root@apache.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-nutch/refs/heads/main/security/apache-nutch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web Crawler
- Indexing
- Search
- Apache
- Java
- Hadoop
- Open Source
---
