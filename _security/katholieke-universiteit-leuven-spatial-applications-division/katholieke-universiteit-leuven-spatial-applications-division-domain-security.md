---
description: ''
domains:
- caa:
  - 0 issue "harica.gr"
  - 0 iodef "mailto:abuse@kuleuven.be"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kuleuven.be
  spf: true
hosts:
- host: www.sadl.kuleuven.be
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Katholieke Universiteit Leuven Spatial Applications Division Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Katholieke Universiteit Leuven, Spatial Applications Division, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Katholieke Universiteit Leuven, Spatial Applications Division
provider_slug: katholieke-universiteit-leuven-spatial-applications-division
slug: katholieke-universiteit-leuven-spatial-applications-division-domain-security
source_filename: katholieke-universiteit-leuven-spatial-applications-division-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sadl.kuleuven.be\n  https: false\ndomains:\n- domain: kuleuven.be\n  dnssec: false\n  caa:\n  - 0 issue \"harica.gr\"\n  - 0 iodef \"mailto:abuse@kuleuven.be\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/katholieke-universiteit-leuven-spatial-applications-division/security/katholieke-universiteit-leuven-spatial-applications-division-domain-security.yml
summary_line: DMARC
tags:
- Company
- Research
- Education
- Geospatial
- Consultancy
---
