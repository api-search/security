---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tum.de
  spf: true
hosts:
- cert_expires: Jan 11 16:35:23 2027 GMT
  host: www.tum.de
  hsts: true
  hsts_max_age: 86400000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Technische Universit T M Nchen Runder Tisch Gis E V Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Technische Universität München - Runder Tisch GIS e.V., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Technische Universität München - Runder Tisch GIS e.V.
provider_slug: technische-universit-t-m-nchen-runder-tisch-gis-e-v
slug: technische-universit-t-m-nchen-runder-tisch-gis-e-v-domain-security
source_filename: technische-universit-t-m-nchen-runder-tisch-gis-e-v-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tum.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 16:35:23 2027 GMT\n  hsts: true\n  hsts_max_age: 86400000\ndomains:\n- domain: tum.de\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/technische-universit-t-m-nchen-runder-tisch-gis-e-v/security/technische-universit-t-m-nchen-runder-tisch-gis-e-v-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- GIS
- Education
- Research
- Open-Source
- Community
- Company
---
