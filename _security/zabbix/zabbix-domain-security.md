---
api_specs:
- filename: zabbix-actions-api-openapi.yml
  format: yaml
  label: Zabbix Actions API
  slug: zabbix-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-actions-api-openapi.yml
- filename: zabbix-authentication-api-openapi.yml
  format: yaml
  label: Zabbix Authentication API
  slug: zabbix-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-authentication-api-openapi.yml
- filename: zabbix-events-api-openapi.yml
  format: yaml
  label: Zabbix Events API
  slug: zabbix-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-events-api-openapi.yml
- filename: zabbix-history-api-openapi.yml
  format: yaml
  label: Zabbix History API
  slug: zabbix-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-history-api-openapi.yml
- filename: zabbix-host-groups-api-openapi.yml
  format: yaml
  label: Zabbix Host Groups API
  slug: zabbix-host-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-host-groups-api-openapi.yml
- filename: zabbix-hosts-api-openapi.yml
  format: yaml
  label: Zabbix Hosts API
  slug: zabbix-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-hosts-api-openapi.yml
- filename: zabbix-items-api-openapi.yml
  format: yaml
  label: Zabbix Items API
  slug: zabbix-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-items-api-openapi.yml
- filename: zabbix-problems-api-openapi.yml
  format: yaml
  label: Zabbix Problems API
  slug: zabbix-problems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-problems-api-openapi.yml
- filename: zabbix-triggers-api-openapi.yml
  format: yaml
  label: Zabbix Triggers API
  slug: zabbix-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-triggers-api-openapi.yml
- filename: zabbix-users-api-openapi.yml
  format: yaml
  label: Zabbix Users API
  slug: zabbix-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zabbix.com
  spf: true
hosts:
- cert_expires: Oct  5 19:22:39 2026 GMT
  host: www.zabbix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zabbix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zabbix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zabbix
provider_slug: zabbix
slug: zabbix-domain-security
source_filename: zabbix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zabbix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 19:22:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zabbix.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/security/zabbix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Monitoring
- Infrastructure
- Networks
- Alerting
- Open-Source
- Observability
---
