---
api_specs:
- filename: pica8-backup-api-openapi.yml
  format: yaml
  label: Pica8 Backup API
  slug: pica8-backup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pica8/refs/heads/main/openapi/pica8-backup-api-openapi.yml
- filename: pica8-configuration-api-openapi.yml
  format: yaml
  label: Pica8 Configuration API
  slug: pica8-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pica8/refs/heads/main/openapi/pica8-configuration-api-openapi.yml
- filename: pica8-configurationfile-api-openapi.yml
  format: yaml
  label: Pica8 Configuration File API
  slug: pica8-configurationfile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pica8/refs/heads/main/openapi/pica8-configurationfile-api-openapi.yml
- filename: pica8-group-api-openapi.yml
  format: yaml
  label: Pica8 Group API
  slug: pica8-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pica8/refs/heads/main/openapi/pica8-group-api-openapi.yml
- filename: pica8-job-api-openapi.yml
  format: yaml
  label: Pica8 Job API
  slug: pica8-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pica8/refs/heads/main/openapi/pica8-job-api-openapi.yml
- filename: pica8-license-api-openapi.yml
  format: yaml
  label: Pica8 License API
  slug: pica8-license-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pica8/refs/heads/main/openapi/pica8-license-api-openapi.yml
- filename: pica8-playbook-api-openapi.yml
  format: yaml
  label: Pica8 Playbook API
  slug: pica8-playbook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pica8/refs/heads/main/openapi/pica8-playbook-api-openapi.yml
- filename: pica8-settings-api-openapi.yml
  format: yaml
  label: Pica8 Settings API
  slug: pica8-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pica8/refs/heads/main/openapi/pica8-settings-api-openapi.yml
- filename: pica8-switch-api-openapi.yml
  format: yaml
  label: Pica8 Switch API
  slug: pica8-switch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pica8/refs/heads/main/openapi/pica8-switch-api-openapi.yml
- filename: pica8-template-api-openapi.yml
  format: yaml
  label: Pica8 Template API
  slug: pica8-template-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pica8/refs/heads/main/openapi/pica8-template-api-openapi.yml
- filename: pica8-token-api-openapi.yml
  format: yaml
  label: Pica8 Token API
  slug: pica8-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pica8/refs/heads/main/openapi/pica8-token-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pica8.com
  spf: true
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: atlassian.net
  spf: true
hosts:
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: www.pica8.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: pica8-fs.atlassian.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pica8 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pica8, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pica8
provider_slug: pica8
slug: pica8-domain-security
source_filename: pica8-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pica8.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: pica8-fs.atlassian.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pica8.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: atlassian.net\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com; account=c2eb0f50ca113d7543d58a10f523d0469ff922f115e5e4e9056f3d5f87d3356c\"\n  spf: true\n  dmarc: true\n\
  \  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pica8/refs/heads/main/security/pica8-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Networking
- Open Networking
- Software Defined Networking
- Network Automation
- Network Operating System
- white-box-switching
- Network Management
- Campus Networking
- Data Center Networking
- RESTCONF
- NETCONF
- Telemetry
---
