---
api_specs:
- filename: apache-tika-apache-tika-server-rest-api-api-openapi.yml
  format: yaml
  label: Apache Tika Apache Tika Server REST API API
  slug: apache-tika-apache-tika-server-rest-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-tika/refs/heads/main/openapi/apache-tika-apache-tika-server-rest-api-api-openapi.yml
- filename: apache-tika-detect-api-openapi.yml
  format: yaml
  label: Apache Tika Detect API
  slug: apache-tika-detect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-tika/refs/heads/main/openapi/apache-tika-detect-api-openapi.yml
- filename: apache-tika-detectors-api-openapi.yml
  format: yaml
  label: Apache Tika Detectors API
  slug: apache-tika-detectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-tika/refs/heads/main/openapi/apache-tika-detectors-api-openapi.yml
- filename: apache-tika-language-api-openapi.yml
  format: yaml
  label: Apache Tika Language API
  slug: apache-tika-language-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-tika/refs/heads/main/openapi/apache-tika-language-api-openapi.yml
- filename: apache-tika-meta-api-openapi.yml
  format: yaml
  label: Apache Tika Meta API
  slug: apache-tika-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-tika/refs/heads/main/openapi/apache-tika-meta-api-openapi.yml
- filename: apache-tika-mime-types-api-openapi.yml
  format: yaml
  label: Apache Tika Mime Types API
  slug: apache-tika-mime-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-tika/refs/heads/main/openapi/apache-tika-mime-types-api-openapi.yml
- filename: apache-tika-parsers-api-openapi.yml
  format: yaml
  label: Apache Tika Parsers API
  slug: apache-tika-parsers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-tika/refs/heads/main/openapi/apache-tika-parsers-api-openapi.yml
- filename: apache-tika-rmeta-api-openapi.yml
  format: yaml
  label: Apache Tika Rmeta API
  slug: apache-tika-rmeta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-tika/refs/heads/main/openapi/apache-tika-rmeta-api-openapi.yml
- filename: apache-tika-status-api-openapi.yml
  format: yaml
  label: Apache Tika Status API
  slug: apache-tika-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-tika/refs/heads/main/openapi/apache-tika-status-api-openapi.yml
- filename: apache-tika-tika-api-openapi.yml
  format: yaml
  label: Apache Tika Tika API
  slug: apache-tika-tika-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-tika/refs/heads/main/openapi/apache-tika-tika-api-openapi.yml
- filename: apache-tika-translate-api-openapi.yml
  format: yaml
  label: Apache Tika Translate API
  slug: apache-tika-translate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-tika/refs/heads/main/openapi/apache-tika-translate-api-openapi.yml
- filename: apache-tika-unpack-api-openapi.yml
  format: yaml
  label: Apache Tika Unpack API
  slug: apache-tika-unpack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-tika/refs/heads/main/openapi/apache-tika-unpack-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:root@apache.org"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apache.org
  spf: true
hosts:
- cert_expires: Aug 24 23:33:10 2026 GMT
  host: tika.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 04:10:25 2026 GMT
  host: cwiki.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apache Tika Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache Tika, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apache Tika
provider_slug: apache-tika
slug: apache-tika-domain-security
source_filename: apache-tika-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tika.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cwiki.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 04:10:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:root@apache.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-tika/refs/heads/main/security/apache-tika-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Content Extraction
- Document Processing
- Metadata
- Text Extraction
- Open Source
---
