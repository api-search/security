---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Allego API
  slug: allego-api
  spec_type: OpenAPI
  url: https://exp-build.allego.com/api/
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 issue ";"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: allego.com
  spf: true
hosts:
- cert_expires: Sep 15 19:24:25 2026 GMT
  host: www.allego.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: exp-build.allego.com
  https: false
kind: domain-security
layout: security
method: probed
name: Allego Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Allego, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Allego
provider_slug: allego
slug: allego-domain-security
source_filename: allego-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.allego.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 19:24:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: exp-build.allego.com\n  https: false\ndomains:\n- domain: allego.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \";\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allego/refs/heads/main/security/allego-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sales Enablement
- Sales Training
- Video Coaching
- Content Management
- Conversation Intelligence
- Deal Intelligence
- Revenue Enablement
- Certifications
- AI
---
