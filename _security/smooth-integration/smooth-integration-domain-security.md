---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: smooth-integration.com
  spf: false
hosts:
- host: smooth-integration.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Smooth Integration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smooth Integration, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Smooth Integration
provider_slug: smooth-integration
slug: smooth-integration-domain-security
source_filename: smooth-integration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smooth-integration.com\n  https: false\ndomains:\n- domain: smooth-integration.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/smooth-integration/security/smooth-integration-domain-security.yml
summary_line: DMARC
tags:
- Integration
- Middleware
- Automation
- Enterprise
---
