---
api_specs:
- filename: apache-apisix-consumer-groups-api-openapi.yml
  format: yaml
  label: Apache APISIX Consumer Groups API
  slug: apache-apisix-consumer-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-consumer-groups-api-openapi.yml
- filename: apache-apisix-consumers-api-openapi.yml
  format: yaml
  label: Apache APISIX Consumers API
  slug: apache-apisix-consumers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-consumers-api-openapi.yml
- filename: apache-apisix-diagnostics-api-openapi.yml
  format: yaml
  label: Apache APISIX Diagnostics API
  slug: apache-apisix-diagnostics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-diagnostics-api-openapi.yml
- filename: apache-apisix-global-rules-api-openapi.yml
  format: yaml
  label: Apache APISIX Global Rules API
  slug: apache-apisix-global-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-global-rules-api-openapi.yml
- filename: apache-apisix-health-check-api-openapi.yml
  format: yaml
  label: Apache APISIX Health Check API
  slug: apache-apisix-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-health-check-api-openapi.yml
- filename: apache-apisix-introspection-api-openapi.yml
  format: yaml
  label: Apache APISIX Introspection API
  slug: apache-apisix-introspection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-introspection-api-openapi.yml
- filename: apache-apisix-plugin-configs-api-openapi.yml
  format: yaml
  label: Apache APISIX Plugin Configs API
  slug: apache-apisix-plugin-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-plugin-configs-api-openapi.yml
- filename: apache-apisix-plugin-metadata-api-openapi.yml
  format: yaml
  label: Apache APISIX Plugin Metadata API
  slug: apache-apisix-plugin-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-plugin-metadata-api-openapi.yml
- filename: apache-apisix-plugins-api-openapi.yml
  format: yaml
  label: Apache APISIX Plugins API
  slug: apache-apisix-plugins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-plugins-api-openapi.yml
- filename: apache-apisix-protos-api-openapi.yml
  format: yaml
  label: Apache APISIX Protos API
  slug: apache-apisix-protos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-protos-api-openapi.yml
- filename: apache-apisix-routes-api-openapi.yml
  format: yaml
  label: Apache APISIX Routes API
  slug: apache-apisix-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-routes-api-openapi.yml
- filename: apache-apisix-schema-api-openapi.yml
  format: yaml
  label: Apache APISIX Schema API
  slug: apache-apisix-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-schema-api-openapi.yml
- filename: apache-apisix-secrets-api-openapi.yml
  format: yaml
  label: Apache APISIX Secrets API
  slug: apache-apisix-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-secrets-api-openapi.yml
- filename: apache-apisix-services-api-openapi.yml
  format: yaml
  label: Apache APISIX Services API
  slug: apache-apisix-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-services-api-openapi.yml
- filename: apache-apisix-ssl-api-openapi.yml
  format: yaml
  label: Apache APISIX SSL API
  slug: apache-apisix-ssl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-ssl-api-openapi.yml
- filename: apache-apisix-stream-routes-api-openapi.yml
  format: yaml
  label: Apache APISIX Stream Routes API
  slug: apache-apisix-stream-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-stream-routes-api-openapi.yml
- filename: apache-apisix-upstreams-api-openapi.yml
  format: yaml
  label: Apache APISIX Upstreams API
  slug: apache-apisix-upstreams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-apisix/refs/heads/main/openapi/apache-apisix-upstreams-api-openapi.yml
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
