---
description: ''
domains:
- caa:
  - 0 issue "certificados.serpro.gov.br"
  - 0 issue "globalsign.com"
  - 0 issue "digicert.com"
  - 0 iodef "mailto:csirt@bcb.gov.br"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bcb.gov.br
  spf: true
hosts:
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: dadosabertos.bcb.gov.br
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brazil Central Bank Open Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brazil Central Bank Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Brazil Central Bank Open Data
provider_slug: brazil-central-bank-open-data
slug: brazil-central-bank-open-data-domain-security
source_filename: brazil-central-bank-open-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dadosabertos.bcb.gov.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: bcb.gov.br\n  dnssec: false\n  caa:\n  - 0 issue \"certificados.serpro.gov.br\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:csirt@bcb.gov.br\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brazil-central-bank-open-data/refs/heads/main/security/brazil-central-bank-open-data-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Government
- Public APIs
---
