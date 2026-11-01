---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: meteoromania.ro
  spf: true
hosts:
- cert_expires: Apr 12 23:59:59 2027 GMT
  host: www.meteoromania.ro
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: National Meteorological Administration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Meteorological Administration, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: National Meteorological Administration
provider_slug: national-meteorological-administration
slug: national-meteorological-administration-domain-security
source_filename: national-meteorological-administration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.meteoromania.ro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 12 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: meteoromania.ro\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/national-meteorological-administration/security/national-meteorological-administration-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
---
