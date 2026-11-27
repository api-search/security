---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ileza.pl
  spf: true
hosts:
- cert_expires: Jan 19 15:19:45 2027 GMT
  host: ileza.pl
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: IleZa.pl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IleZa.pl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: IleZa.pl
provider_slug: ileza-pl
slug: ileza-pl-domain-security
source_filename: ileza-pl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ileza.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 15:19:45 2027 GMT\n  hsts: false\ndomains:\n- domain: ileza.pl\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ileza-pl/security/ileza-pl-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Price Comparison
- Consumer Finance
- Poland
- Open Data
---
