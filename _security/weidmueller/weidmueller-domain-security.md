---
api_specs:
- filename: weidmueller-variable-nats-asyncapi.yml
  format: yaml
  label: Weidmüller u-OS Data Hub Variable-NATS API
  slug: u-os-data-hub-variable-nats-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/asyncapi/weidmueller-variable-nats-asyncapi.yml
- filename: weidmueller-consumer-api-openapi.yml
  format: yaml
  label: Weidmüller Consumer API
  slug: weidmueller-consumer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-consumer-api-openapi.yml
- filename: weidmueller-firewall-api-openapi.yml
  format: yaml
  label: Weidmüller Firewall API
  slug: weidmueller-firewall-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-firewall-api-openapi.yml
- filename: weidmueller-logging-api-openapi.yml
  format: yaml
  label: Weidmüller Logging API
  slug: weidmueller-logging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-logging-api-openapi.yml
- filename: weidmueller-network-api-openapi.yml
  format: yaml
  label: Weidmüller Network API
  slug: weidmueller-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-network-api-openapi.yml
- filename: weidmueller-operations-api-openapi.yml
  format: yaml
  label: Weidmüller Operations API
  slug: weidmueller-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-operations-api-openapi.yml
- filename: weidmueller-ping-api-openapi.yml
  format: yaml
  label: Weidmüller Ping API
  slug: weidmueller-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-ping-api-openapi.yml
- filename: weidmueller-realtime-api-openapi.yml
  format: yaml
  label: Weidmüller Realtime API
  slug: weidmueller-realtime-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-realtime-api-openapi.yml
- filename: weidmueller-recovery-api-openapi.yml
  format: yaml
  label: Weidmüller Recovery API
  slug: weidmueller-recovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-recovery-api-openapi.yml
- filename: weidmueller-security-api-openapi.yml
  format: yaml
  label: Weidmüller Security API
  slug: weidmueller-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-security-api-openapi.yml
- filename: weidmueller-serial-interfaces-api-openapi.yml
  format: yaml
  label: Weidmüller Serial Interfaces API
  slug: weidmueller-serial-interfaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-serial-interfaces-api-openapi.yml
- filename: weidmueller-syslog-api-openapi.yml
  format: yaml
  label: Weidmüller Syslog API
  slug: weidmueller-syslog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-syslog-api-openapi.yml
- filename: weidmueller-system-api-openapi.yml
  format: yaml
  label: Weidmüller System API
  slug: weidmueller-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-system-api-openapi.yml
- filename: weidmueller-time-api-openapi.yml
  format: yaml
  label: Weidmüller Time API
  slug: weidmueller-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-time-api-openapi.yml
- filename: weidmueller-update-api-openapi.yml
  format: yaml
  label: Weidmüller Update API
  slug: weidmueller-update-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-update-api-openapi.yml
- filename: weidmueller-open-api-api-openapi.yml
  format: yaml
  label: Weidmüller Open API
  slug: weidmueller-open-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/openapi/weidmueller-open-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: weidmueller.com
  spf: true
hosts:
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: www.weidmueller.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Weidmueller Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Weidmüller, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Weidmüller
provider_slug: weidmueller
slug: weidmueller-domain-security
source_filename: weidmueller-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.weidmueller.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: weidmueller.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weidmueller/refs/heads/main/security/weidmueller-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Industrial Automation
- Industrial Connectivity
- Edge Computing
- IIoT
- u-OS
- Manufacturing
---
