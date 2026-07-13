---
api_specs:
- filename: apache-apisix-admin-api-openapi.yml
  format: yaml
  label: Apache APISIX Admin API
  slug: apache-apisix-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-admin-api-openapi.yml
- filename: apache-apisix-control-api-openapi.yml
  format: yaml
  label: Apache APISIX Control API
  slug: apache-apisix-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-control-api-openapi.yml
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
  host: apisix.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: 127.0.0.1
  https: false
kind: domain-security
layout: security
method: probed
name: Apache Apisix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache APISIX, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apache APISIX
provider_slug: apache-apisix
slug: apache-apisix-domain-security
source_filename: apache-apisix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apisix.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: 127.0.0.1\n  https: false\ndomains:\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:root@apache.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/security/apache-apisix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apache
- API Gateway
- Cloud Native
- Kubernetes
- Lua
- NGINX
- Open Source
- Traffic Management
---
