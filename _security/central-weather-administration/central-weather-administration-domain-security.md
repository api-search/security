---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cwa.gov.tw
  spf: true
hosts:
- host: cwa.gov.tw
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Central Weather Administration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CWA (Taiwan), probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: CWA (Taiwan)
provider_slug: central-weather-administration
slug: central-weather-administration-domain-security
source_filename: central-weather-administration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cwa.gov.tw\n  https: false\ndomains:\n- domain: cwa.gov.tw\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/central-weather-administration/security/central-weather-administration-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
---
