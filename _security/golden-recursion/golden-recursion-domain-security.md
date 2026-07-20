---
api_specs:
- filename: golden-recursion-openapi-original.json
  format: json
  label: Golden API v2
  slug: golden-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/golden-recursion/refs/heads/main/openapi/golden-recursion-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:hello@golden-support.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: golden.com
  spf: true
hosts:
- cert_expires: Aug 25 07:32:13 2026 GMT
  host: golden.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Golden Recursion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Golden Recursion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Golden Recursion
provider_slug: golden-recursion
slug: golden-recursion-domain-security
source_filename: golden-recursion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: golden.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 07:32:13 2026 GMT\n  hsts: false\ndomains:\n- domain: golden.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:hello@golden-support.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/golden-recursion/refs/heads/main/security/golden-recursion-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Knowledge Graph
- Data Enrichment
- Entity Data
- Company Data
- Artificial Intelligence
- Semantic Web
- Data
---
