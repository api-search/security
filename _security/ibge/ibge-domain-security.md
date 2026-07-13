---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ibge.gov.br
  spf: true
hosts:
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: servicodados.ibge.gov.br
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ibge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IBGE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: IBGE
provider_slug: ibge
slug: ibge-domain-security
source_filename: ibge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: servicodados.ibge.gov.br\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: ibge.gov.br\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ibge/refs/heads/main/security/ibge-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Geocoding
- Public APIs
---
