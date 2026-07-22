---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rebajatuscuentas.com
  spf: true
hosts:
- cert_expires: Sep  5 05:20:16 2026 GMT
  host: rebajatuscuentas.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rebaja Tus Cuentas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rebaja Tus Cuentas, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rebaja Tus Cuentas
provider_slug: rebaja-tus-cuentas
slug: rebaja-tus-cuentas-domain-security
source_filename: rebaja-tus-cuentas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rebajatuscuentas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 05:20:16 2026 GMT\n  hsts: false\ndomains:\n- domain: rebajatuscuentas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rebaja-tus-cuentas/refs/heads/main/security/rebaja-tus-cuentas-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Consumer Finance
- Lending
- Debt Refinancing
- Personal Finance
- Latin America
- Peru
---
