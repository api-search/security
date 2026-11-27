---
api_specs:
- filename: mandiant-projects-api-openapi.yml
  format: yaml
  label: Mandiant Projects API
  slug: mandiant-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mandiant/openapi/mandiant-projects-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: false
  dnssec: true
  domain: mandiant.com
  spf: true
hosts:
- cert_expires: Feb  9 05:27:26 2027 GMT
  host: mandiant.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  9 05:27:26 2027 GMT
  host: docs.mandiant.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 21 11:47:50 2026 GMT
  host: api.intelligence.mandiant.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Mandiant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mandiant, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Mandiant
provider_slug: mandiant
slug: mandiant-domain-security
source_filename: mandiant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mandiant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 05:27:26 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.mandiant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 05:27:26 2027 GMT\n  hsts: false\n- host: api.intelligence.mandiant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 11:47:50 2026 GMT\n  hsts: null\ndomains:\n- domain: mandiant.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mandiant/security/mandiant-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Security
- Threat Intelligence
- Cybersecurity
- Incident Response
- Attack Surface Management
- Vulnerability Intelligence
- Malware
- Google Cloud
---
