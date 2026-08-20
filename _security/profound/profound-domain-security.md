---
api_specs:
- filename: profound-external-api-openapi.json
  format: json
  label: Profound External API
  slug: profound-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/openapi/profound-external-api-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: tryprofound.com
  spf: true
hosts:
- cert_expires: Nov  6 05:19:15 2026 GMT
  host: www.tryprofound.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 20:14:00 2026 GMT
  host: api.tryprofound.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Profound Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Profound, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Profound
provider_slug: profound
slug: profound-domain-security
source_filename: profound-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tryprofound.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 05:19:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tryprofound.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 20:14:00 2026 GMT\n  hsts: null\ndomains:\n- domain: tryprofound.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/profound/refs/heads/main/security/profound-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Answer Engine Optimization
- AEO
- AI Search
- Generative Engine Optimization
- Marketing
- Analytics
- Agent Analytics
- Brand Visibility
- Citations
- MCP
---
