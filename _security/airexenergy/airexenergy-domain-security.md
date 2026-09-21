---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: airex-energy.com
  spf: true
hosts:
- host: airex-energy.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Airexenergy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airex Energy, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Airex Energy
provider_slug: airexenergy
slug: airexenergy-domain-security
source_filename: airexenergy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: airex-energy.com\n  https: false\ndomains:\n- domain: airex-energy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nnote: 'The TLS/HTTP leg of this probe ran while the airex-energy.com origin (51.79.107.79)\n  had stopped answering on port 443 mid-pass; hosts[0].https: false is that outage,\n  not a missing certificate. Earlier in the same run the apex answered HTTP 200 over\n  HTTPS and www.airex-energy.com 301-redirected to it. The DNS findings (DNSSEC absent,\n  no CAA, SPF and DMARC published with p=quarantine) are unaffected.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airexenergy/refs/heads/main/security/airexenergy-domain-security.yml
summary_line: DMARC
tags:
- Company
- Biochar
- Biocoal
- Bioenergy
- Torrefaction
- Carbon Removal
- Clean Technology
- Biomass
- Manufacturing
---
