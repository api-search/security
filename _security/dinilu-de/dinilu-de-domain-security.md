---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dinilu.de
  spf: true
hosts:
- cert_expires: Jan  5 06:17:43 2027 GMT
  host: dinilu.de
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dinilu De Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dinilu Werbe- & Druckartikel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Dinilu Werbe- & Druckartikel
provider_slug: dinilu-de
slug: dinilu-de-domain-security
source_filename: dinilu-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dinilu.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 06:17:43 2027 GMT\n  hsts: null\ndomains:\n- domain: dinilu.de\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/dinilu-de/security/dinilu-de-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Advertising
- Printing
- Wholesale
- Europe
- E-Commerce
- Company
---
