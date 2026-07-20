---
api_specs:
- filename: codesphere-openapi-original.json
  format: json
  label: Codesphere Public API
  slug: codesphere-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/codesphere/refs/heads/main/openapi/codesphere-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: codesphere.com
  spf: true
hosts:
- cert_expires: Aug 18 13:45:49 2026 GMT
  host: codesphere.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 12:28:40 2026 GMT
  host: cloud.codesphere.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Codesphere Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Codesphere, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Codesphere
provider_slug: codesphere
slug: codesphere-domain-security
source_filename: codesphere-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codesphere.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 13:45:49 2026 GMT\n  hsts: false\n- host: cloud.codesphere.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 12:28:40 2026 GMT\n  hsts: false\ndomains:\n- domain: codesphere.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codesphere/refs/heads/main/security/codesphere-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Saas
- Cloud
- Deployment
- Developer Tools
- Platform as a Service
- Infrastructure
- Sovereign Cloud
- CI/CD
- Managed Services
---
