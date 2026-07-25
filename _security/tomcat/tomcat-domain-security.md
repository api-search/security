---
api_specs:
- filename: tomcat-applications-api-openapi.yml
  format: yaml
  label: Apache Tomcat Applications API
  slug: tomcat-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomcat/refs/heads/main/openapi/tomcat-applications-api-openapi.yml
- filename: tomcat-configuration-api-openapi.yml
  format: yaml
  label: Apache Tomcat Configuration API
  slug: tomcat-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomcat/refs/heads/main/openapi/tomcat-configuration-api-openapi.yml
- filename: tomcat-diagnostics-api-openapi.yml
  format: yaml
  label: Apache Tomcat Diagnostics API
  slug: tomcat-diagnostics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomcat/refs/heads/main/openapi/tomcat-diagnostics-api-openapi.yml
- filename: tomcat-jmx-api-openapi.yml
  format: yaml
  label: Apache Tomcat JMX API
  slug: tomcat-jmx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomcat/refs/heads/main/openapi/tomcat-jmx-api-openapi.yml
- filename: tomcat-sessions-api-openapi.yml
  format: yaml
  label: Apache Tomcat Sessions API
  slug: tomcat-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomcat/refs/heads/main/openapi/tomcat-sessions-api-openapi.yml
- filename: tomcat-ssl-api-openapi.yml
  format: yaml
  label: Apache Tomcat SSL API
  slug: tomcat-ssl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomcat/refs/heads/main/openapi/tomcat-ssl-api-openapi.yml
- filename: tomcat-status-api-openapi.yml
  format: yaml
  label: Apache Tomcat Status API
  slug: tomcat-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomcat/refs/heads/main/openapi/tomcat-status-api-openapi.yml
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
  host: tomcat.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tomcat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apache Tomcat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Apache Tomcat
provider_slug: tomcat
slug: tomcat-domain-security
source_filename: tomcat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tomcat.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apache.org\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:root@apache.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tomcat/refs/heads/main/security/tomcat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Application Server
- Java
- Servlet Container
- Web Server
- Open Source
- Apache
---
