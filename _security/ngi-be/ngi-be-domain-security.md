---
description: ''
domains:
- caa:
  - 0 issue "harica.gr"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ngi.be
  spf: true
hosts:
- cert_expires: Feb 12 10:43:09 2027 GMT
  host: www.ngi.be
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: National Geographic Institute (NGI) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Geographic Institute (NGI), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: National Geographic Institute (NGI)
provider_slug: ngi-be
slug: ngi-be-domain-security
source_filename: ngi-be-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ngi.be\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 10:43:09 2027 GMT\n  hsts: false\ndomains:\n- domain: ngi.be\n  dnssec: true\n  caa:\n  - 0 issue \"harica.gr\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/ngi-be/security/ngi-be-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Government
- Geospatial
- Mapping
- Open Data
- OGC
- Belgium
---
