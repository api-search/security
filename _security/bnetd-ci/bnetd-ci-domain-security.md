---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bnetd.ci
  spf: true
hosts:
- host: bnetd.ci
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bnetd Ci Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bureau National d''Etudes Techniques et de Developpement (BNETD), probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bureau National d'Etudes Techniques et de Developpement (BNETD)
provider_slug: bnetd-ci
slug: bnetd-ci-domain-security
source_filename: bnetd-ci-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bnetd.ci\n  https: false\ndomains:\n- domain: bnetd.ci\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bnetd-ci/security/bnetd-ci-domain-security.yml
summary_line: DMARC
tags:
- Company
- Research
- Development
- France
- Technology
- Engineering
---
