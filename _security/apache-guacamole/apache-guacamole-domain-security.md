---
api_specs:
- filename: apache-guacamole-active-connections-api-openapi.yml
  format: yaml
  label: Apache Guacamole Active Connections API
  slug: apache-guacamole-active-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-guacamole/refs/heads/main/openapi/apache-guacamole-active-connections-api-openapi.yml
- filename: apache-guacamole-authentication-api-openapi.yml
  format: yaml
  label: Apache Guacamole Authentication API
  slug: apache-guacamole-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-guacamole/refs/heads/main/openapi/apache-guacamole-authentication-api-openapi.yml
- filename: apache-guacamole-connections-api-openapi.yml
  format: yaml
  label: Apache Guacamole Connections API
  slug: apache-guacamole-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-guacamole/refs/heads/main/openapi/apache-guacamole-connections-api-openapi.yml
- filename: apache-guacamole-history-api-openapi.yml
  format: yaml
  label: Apache Guacamole History API
  slug: apache-guacamole-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-guacamole/refs/heads/main/openapi/apache-guacamole-history-api-openapi.yml
- filename: apache-guacamole-user-groups-api-openapi.yml
  format: yaml
  label: Apache Guacamole User Groups API
  slug: apache-guacamole-user-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-guacamole/refs/heads/main/openapi/apache-guacamole-user-groups-api-openapi.yml
- filename: apache-guacamole-users-api-openapi.yml
  format: yaml
  label: Apache Guacamole Users API
  slug: apache-guacamole-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apache-guacamole/refs/heads/main/openapi/apache-guacamole-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:root@apache.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apache.org
  spf: true
hosts:
- cert_expires: Aug 24 23:33:10 2026 GMT
  host: guacamole.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apache Guacamole Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache Guacamole, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apache Guacamole
provider_slug: apache-guacamole
slug: apache-guacamole-domain-security
source_filename: apache-guacamole-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: guacamole.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:root@apache.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apache-guacamole/refs/heads/main/security/apache-guacamole-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apache
- Open Source
- RDP
- Remote Access
- Remote Desktop
- SSH
- VNC
- Web Gateway
---
