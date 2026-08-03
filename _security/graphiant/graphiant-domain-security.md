---
api_specs:
- filename: graphiant-portal-openapi-original.json
  format: json
  label: Graphiant Portal REST API
  slug: graphiant-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/graphiant/refs/heads/main/openapi/graphiant-portal-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: graphiant.com
  spf: true
hosts:
- cert_expires: Oct 28 11:44:30 2026 GMT
  host: www.graphiant.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: portal.graphiant.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 18:34:09 2026 GMT
  host: docs.graphiant.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Graphiant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Graphiant, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Graphiant
provider_slug: graphiant
slug: graphiant-domain-security
source_filename: graphiant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.graphiant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 11:44:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal.graphiant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: false\n- host: docs.graphiant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 18:34:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: graphiant.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graphiant/refs/heads/main/security/graphiant-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Networking
- Network as a Service
- NaaS
- Connectivity
- SD-WAN
- Cloud Networking
- Zero Trust
- Network Security
- Data Sovereignty
- Observability
- Infrastructure
- Automation
---
