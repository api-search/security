---
api_specs:
- filename: gouda-studios-agent-tools-openapi.json
  format: json
  label: Gouda Studios Agent Tools API
  slug: gouda-studios-agent-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gouda-studios-agent-tools/openapi/gouda-studios-agent-tools-openapi.json
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vercel.app
  spf: true
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: apify.com
  spf: true
hosts:
- cert_expires: Nov 27 19:48:08 2026 GMT
  host: gouda-studios-agent-tools.vercel.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: api.apify.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Gouda Studios Agent Tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gouda Studios Agent Tools, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gouda Studios Agent Tools
provider_slug: gouda-studios-agent-tools
slug: gouda-studios-agent-tools-domain-security
source_filename: gouda-studios-agent-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gouda-studios-agent-tools.vercel.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 19:48:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.apify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: vercel.app\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: apify.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/gouda-studios-agent-tools/security/gouda-studios-agent-tools-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Data
- Government
- Finance
- API
- Pay-per-result
---
