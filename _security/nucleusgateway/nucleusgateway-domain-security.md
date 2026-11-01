---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nucleusgateway.com
  spf: false
hosts:
- host: nucleusgateway.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nucleusgateway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nucleus AI, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Nucleus AI
provider_slug: nucleusgateway
slug: nucleusgateway-domain-security
source_filename: nucleusgateway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nucleusgateway.com\n  https: false\ndomains:\n- domain: nucleusgateway.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/nucleusgateway/security/nucleusgateway-domain-security.yml
summary_line: DMARC
tags:
- Company
---
