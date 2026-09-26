---
api_specs:
- filename: apsis19b1-openapi-generated.yml
  format: yaml
  label: Apsis19b1 API
  slug: apsis19b1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apsis19b1/refs/heads/main/openapi/_ae-authored/apsis19b1-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:cloudengineers@apsis.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: apsis.com
  spf: true
hosts:
- cert_expires: Dec  3 01:36:13 2026 GMT
  host: www.apsis.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apsis19B1 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apsis19b1, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Apsis19b1
provider_slug: apsis19b1
slug: apsis19b1-domain-security
source_filename: apsis19b1-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apsis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 01:36:13 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: apsis.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:cloudengineers@apsis.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apsis19b1/refs/heads/main/security/apsis19b1-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketing
- Email
- Automation
- AI
- GDPR
---
