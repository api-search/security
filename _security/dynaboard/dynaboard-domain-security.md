---
api_specs:
- filename: dynaboard-openapi-generated.yml
  format: yaml
  label: Dynaboard API
  slug: dynaboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dynaboard/openapi/_ae-authored/dynaboard-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:webmaster@dynaboard.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dynaboard.com
  spf: true
hosts:
- cert_expires: Dec 21 21:44:37 2026 GMT
  host: dynaboard.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dynaboard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dynaboard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Dynaboard
provider_slug: dynaboard
slug: dynaboard-domain-security
source_filename: dynaboard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dynaboard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 21:44:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dynaboard.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:webmaster@dynaboard.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/dynaboard/security/dynaboard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Low-code
- Collaboration
- Real-time
- AI
- Web Development
---
