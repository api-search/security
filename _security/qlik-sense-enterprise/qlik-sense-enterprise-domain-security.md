---
api_specs:
- filename: qlik-sense-enterprise-repository-service-openapi.yml
  format: yaml
  label: Qlik Sense Repository Service
  slug: qlik-sense-repository-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qlik-sense-enterprise/refs/heads/main/openapi/qlik-sense-enterprise-repository-service-openapi.yml
- filename: qlik-sense-enterprise-proxy-service-openapi.yml
  format: yaml
  label: Qlik Sense Proxy Service
  slug: qlik-sense-proxy-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qlik-sense-enterprise/refs/heads/main/openapi/qlik-sense-enterprise-proxy-service-openapi.yml
- filename: qlik-sense-enterprise-about-service-openapi.yml
  format: yaml
  label: Qlik Sense About Service
  slug: qlik-sense-about-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qlik-sense-enterprise/refs/heads/main/openapi/qlik-sense-enterprise-about-service-openapi.yml
- filename: qlik-sense-enterprise-data-connection-openapi.yml
  format: yaml
  label: Qlik Sense Data Connection
  slug: qlik-sense-data-connection
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qlik-sense-enterprise/refs/heads/main/openapi/qlik-sense-enterprise-data-connection-openapi.yml
- filename: qlik-sense-enterprise-licenses-openapi.yml
  format: yaml
  label: Qlik Sense Licenses
  slug: qlik-sense-licenses
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qlik-sense-enterprise/refs/heads/main/openapi/qlik-sense-enterprise-licenses-openapi.yml
- filename: qlik-sense-enterprise-odag-service-openapi.yml
  format: yaml
  label: Qlik Sense ODAG
  slug: qlik-sense-odag
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qlik-sense-enterprise/refs/heads/main/openapi/qlik-sense-enterprise-odag-service-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: qlik.dev
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: qlik.com
  spf: true
hosts:
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: qlik.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 16:03:53 2026 GMT
  host: www.qlik.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  8 23:59:59 2027 GMT
  host: help.qlik.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qlik Sense Enterprise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qlik Sense Enterprise, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Qlik Sense Enterprise
provider_slug: qlik-sense-enterprise
slug: qlik-sense-enterprise-domain-security
source_filename: qlik-sense-enterprise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qlik.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: false\n- host: www.qlik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 16:03:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.qlik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: qlik.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n- domain: qlik.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qlik-sense-enterprise/refs/heads/main/security/qlik-sense-enterprise-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Analytics
- Business Intelligence
- Data Visualization
- Enterprise
- REST API
---
