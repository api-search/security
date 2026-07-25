---
api_specs:
- filename: tufin-compliance-api-openapi.yml
  format: yaml
  label: Tufin Compliance API
  slug: tufin-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/openapi/tufin-compliance-api-openapi.yml
- filename: tufin-devices-api-openapi.yml
  format: yaml
  label: Tufin Devices API
  slug: tufin-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/openapi/tufin-devices-api-openapi.yml
- filename: tufin-objects-api-openapi.yml
  format: yaml
  label: Tufin Objects API
  slug: tufin-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/openapi/tufin-objects-api-openapi.yml
- filename: tufin-revisions-api-openapi.yml
  format: yaml
  label: Tufin Revisions API
  slug: tufin-revisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/openapi/tufin-revisions-api-openapi.yml
- filename: tufin-rules-api-openapi.yml
  format: yaml
  label: Tufin Rules API
  slug: tufin-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/openapi/tufin-rules-api-openapi.yml
- filename: tufin-tasks-api-openapi.yml
  format: yaml
  label: Tufin Tasks API
  slug: tufin-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/openapi/tufin-tasks-api-openapi.yml
- filename: tufin-tickets-api-openapi.yml
  format: yaml
  label: Tufin Tickets API
  slug: tufin-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/openapi/tufin-tickets-api-openapi.yml
- filename: tufin-topology-api-openapi.yml
  format: yaml
  label: Tufin Topology API
  slug: tufin-topology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/openapi/tufin-topology-api-openapi.yml
- filename: tufin-users-api-openapi.yml
  format: yaml
  label: Tufin Users API
  slug: tufin-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/openapi/tufin-users-api-openapi.yml
- filename: tufin-workflow-definitions-api-openapi.yml
  format: yaml
  label: Tufin Workflow Definitions API
  slug: tufin-workflow-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/openapi/tufin-workflow-definitions-api-openapi.yml
- filename: tufin-zones-api-openapi.yml
  format: yaml
  label: Tufin Zones API
  slug: tufin-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/openapi/tufin-zones-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tufin.com
  spf: true
hosts:
- cert_expires: Jul 13 23:59:59 2026 GMT
  host: forum.tufin.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 08:30:26 2026 GMT
  host: www.tufin.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tufin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tufin, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tufin
provider_slug: tufin
slug: tufin-domain-security
source_filename: tufin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forum.tufin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.tufin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:30:26 2026 GMT\n  hsts: false\ndomains:\n- domain: tufin.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tufin/refs/heads/main/security/tufin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Security
- Compliance
- Firewall Management
- Network Security
- Network Topology
- Policy Orchestration
- Risk Management
- Security Policy Management
- Zero Trust
---
