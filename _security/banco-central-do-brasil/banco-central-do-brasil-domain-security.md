---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 iodef "mailto:csirt@bcb.gov.br"
  - 0 issue "certificados.serpro.gov.br"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bcb.gov.br
  spf: true
hosts:
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: www.bcb.gov.br
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Banco Central Do Brasil Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Banco Central do Brasil, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Banco Central do Brasil
provider_slug: banco-central-do-brasil
slug: banco-central-do-brasil-domain-security
source_filename: banco-central-do-brasil-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bcb.gov.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\ndomains:\n- domain: bcb.gov.br\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:csirt@bcb.gov.br\"\n  - 0 issue \"certificados.serpro.gov.br\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/banco-central-do-brasil/refs/heads/main/security/banco-central-do-brasil-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Finance
- Banking
- CentralBank
- Brazil
---
