---
api_specs:
- filename: tenable-vulnerability-management-openapi.json
  format: json
  label: Tenable Vulnerability Management API
  slug: tenable-vulnerability-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenable/refs/heads/main/openapi/tenable-vulnerability-management-openapi.json
- filename: tenable-web-app-scanning-openapi.json
  format: json
  label: Tenable Web Application Scanning API
  slug: tenable-web-application-scanning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenable/refs/heads/main/openapi/tenable-web-app-scanning-openapi.json
- filename: tenable-exposure-management-openapi.json
  format: json
  label: Tenable Exposure Management API
  slug: tenable-exposure-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenable/refs/heads/main/openapi/tenable-exposure-management-openapi.json
- filename: tenable-tenable-platform-settings-openapi.json
  format: json
  label: Tenable Platform & Settings API
  slug: tenable-platform-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenable/refs/heads/main/openapi/tenable-tenable-platform-settings-openapi.json
- filename: tenable-pci-asv-openapi.json
  format: json
  label: Tenable PCI ASV API
  slug: tenable-pci-asv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenable/refs/heads/main/openapi/tenable-pci-asv-openapi.json
- filename: tenable-mssp-openapi.json
  format: json
  label: Tenable MSSP Portal API
  slug: tenable-mssp-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenable/refs/heads/main/openapi/tenable-mssp-openapi.json
- filename: tenable-identity-exposure-openapi.json
  format: json
  label: Tenable Identity Exposure API
  slug: tenable-identity-exposure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenable/refs/heads/main/openapi/tenable-identity-exposure-openapi.json
- filename: tenable-downloads-api-openapi.json
  format: json
  label: Tenable Downloads API
  slug: tenable-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tenable/refs/heads/main/openapi/tenable-downloads-api-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "ssl.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: tenable.com
  spf: true
hosts:
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: www.tenable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 13:42:24 2026 GMT
  host: cloud.tenable.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tenable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tenable, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Tenable
provider_slug: tenable
slug: tenable-domain-security
source_filename: tenable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tenable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud.tenable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 13:42:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tenable.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tenable/refs/heads/main/security/tenable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Enterprise
- Cybersecurity
- Vulnerability Management
- Exposure Management
- Security
- Cloud Security
- Attack Surface Management
---
