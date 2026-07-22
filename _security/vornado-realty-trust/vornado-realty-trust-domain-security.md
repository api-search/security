---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vno.com
  spf: true
hosts:
- cert_expires: Aug 27 00:09:19 2026 GMT
  host: www.vno.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Vornado Realty Trust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vornado Realty Trust, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vornado Realty Trust
provider_slug: vornado-realty-trust
slug: vornado-realty-trust-domain-security
source_filename: vornado-realty-trust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vno.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 27 00:09:19 2026 GMT\n  hsts: false\ndomains:\n- domain: vno.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vornado-realty-trust/refs/heads/main/security/vornado-realty-trust-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Commercial Real Estate
- Fortune 500
- New York City
- REIT
- Real Estate
---
