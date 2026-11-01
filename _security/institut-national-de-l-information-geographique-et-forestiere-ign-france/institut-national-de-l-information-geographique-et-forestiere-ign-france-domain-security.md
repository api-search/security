---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ign.fr
  spf: true
hosts:
- cert_expires: Jan  4 03:30:20 2027 GMT
  host: www.ign.fr
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Institut National De L Information Geographique Et Forestiere Ign France Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Institut National de l''information geographique et forestiere (IGN - France), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Institut National de l'information geographique et forestiere (IGN - France)
provider_slug: institut-national-de-l-information-geographique-et-forestiere-ign-france
slug: institut-national-de-l-information-geographique-et-forestiere-ign-france-domain-security
source_filename: institut-national-de-l-information-geographique-et-forestiere-ign-france-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ign.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 03:30:20 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: ign.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/institut-national-de-l-information-geographique-et-forestiere-ign-france/security/institut-national-de-l-information-geographique-et-forestiere-ign-france-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mapping
- Geospatial
- Data
- France
---
