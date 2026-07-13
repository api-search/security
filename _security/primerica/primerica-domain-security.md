---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: primerica.com
  spf: true
hosts:
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: www.primerica.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- host: developer.primerica.com
  https: false
- host: api.primerica.com
  https: false
kind: domain-security
layout: security
method: probed
name: Primerica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Primerica, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Primerica
provider_slug: primerica
slug: primerica-domain-security
source_filename: primerica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.primerica.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: false\n- host: developer.primerica.com\n  https: false\n- host: api.primerica.com\n  https: false\ndomains:\n- domain: primerica.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/primerica/refs/heads/main/security/primerica-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Insurance
- Financial Services
- Life Insurance
---
