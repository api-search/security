---
api_specs:
- filename: intodns-ai-ai-api-openapi.yml
  format: yaml
  label: IntoDNS.ai AI API
  slug: intodns-ai-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intodns-ai/openapi/intodns-ai-ai-api-openapi.yml
- filename: intodns-ai-dns-api-openapi.yml
  format: yaml
  label: IntoDNS.ai Dns API
  slug: intodns-ai-dns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intodns-ai/openapi/intodns-ai-dns-api-openapi.yml
- filename: intodns-ai-email-api-openapi.yml
  format: yaml
  label: IntoDNS.ai Email API
  slug: intodns-ai-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intodns-ai/openapi/intodns-ai-email-api-openapi.yml
- filename: intodns-ai-scan-api-openapi.yml
  format: yaml
  label: IntoDNS.ai Scan API
  slug: intodns-ai-scan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intodns-ai/openapi/intodns-ai-scan-api-openapi.yml
- filename: intodns-ai-system-api-openapi.yml
  format: yaml
  label: IntoDNS.ai System API
  slug: intodns-ai-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intodns-ai/openapi/intodns-ai-system-api-openapi.yml
- filename: intodns-ai-web-api-openapi.yml
  format: yaml
  label: IntoDNS.ai Web API
  slug: intodns-ai-web-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intodns-ai/openapi/intodns-ai-web-api-openapi.yml
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
  dmarc_policy: reject
  dnssec: true
  domain: intodns.ai
  spf: true
hosts:
- cert_expires: Jan 21 20:51:18 2027 GMT
  host: intodns.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: IntoDNS.ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IntoDNS.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: IntoDNS.ai
provider_slug: intodns-ai
slug: intodns-ai-domain-security
source_filename: intodns-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: intodns.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 20:51:18 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: intodns.ai\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/intodns-ai/security/intodns-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- DNS
- Email Security
- Artificial Intelligence
---
