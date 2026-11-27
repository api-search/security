---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lanetti.fi
  spf: true
hosts:
- host: lanetti.fi
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: lanetti-fi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for lanetti-fi, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: lanetti-fi
provider_slug: lanetti-fi
slug: lanetti-fi-domain-security
source_filename: lanetti-fi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lanetti.fi\n  https: false\ndomains:\n- domain: lanetti.fi\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lanetti-fi/security/lanetti-fi-domain-security.yml
summary_line: DMARC
tags:
- Company
---
