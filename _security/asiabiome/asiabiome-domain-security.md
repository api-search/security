---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: civetbio.com
  spf: true
hosts:
- host: civetbio.com
  https: false
kind: domain-security
layout: security
method: probed
name: Asiabiome Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Asiabiome, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Asiabiome
provider_slug: asiabiome
slug: asiabiome-domain-security
source_filename: asiabiome-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: civetbio.com\n  https: false\ndomains:\n- domain: civetbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asiabiome/refs/heads/main/security/asiabiome-domain-security.yml
summary_line: DMARC
tags:
- Company
---
