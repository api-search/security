---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getfestivo.com
  spf: true
hosts:
- host: docs.getfestivo.com
  https: false
kind: domain-security
layout: security
method: probed
name: Festivo Public Holidays Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Festivo Public Holidays, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Festivo Public Holidays
provider_slug: festivo-public-holidays
slug: festivo-public-holidays-domain-security
source_filename: festivo-public-holidays-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.getfestivo.com\n  https: false\ndomains:\n- domain: getfestivo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/festivo-public-holidays/refs/heads/main/security/festivo-public-holidays-domain-security.yml
summary_line: DMARC
tags:
- Calendar
- Public APIs
---
