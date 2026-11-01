---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: centurioncares.com
  spf: true
hosts:
- host: centurioncares.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Centurioncares Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CenturionCARES, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CenturionCARES
provider_slug: centurioncares
slug: centurioncares-domain-security
source_filename: centurioncares-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: centurioncares.com\n  https: false\ndomains:\n- domain: centurioncares.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/centurioncares/security/centurioncares-domain-security.yml
summary_line: DMARC
tags:
- Company
- HealthTech
- RemoteMonitoring
- Telehealth
- PatientCare
---
