---
api_specs:
- filename: lamatic-openapi-generated.yml
  format: yaml
  label: Lamatic API
  slug: lamatic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lamatic/openapi/_ae-authored/lamatic-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "cname.vercel-dns.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lamatic.ai
  spf: true
hosts:
- cert_expires: Jan 17 12:48:38 2027 GMT
  host: lamatic.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lamatic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lamatic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Lamatic
provider_slug: lamatic
slug: lamatic-domain-security
source_filename: lamatic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lamatic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 12:48:38 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lamatic.ai\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"cname.vercel-dns.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/lamatic/security/lamatic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Middleware
- Generative AI
- Serverless deployment
- Integration
- Software-as-a-Service
- Enterprise
- Agency
---
