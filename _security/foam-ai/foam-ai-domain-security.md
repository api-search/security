---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: foam.ai
  spf: true
hosts:
- host: foam.ai
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: foam-ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for foam-ai, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: foam-ai
provider_slug: foam-ai
slug: foam-ai-domain-security
source_filename: foam-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: foam.ai\n  https: false\ndomains:\n- domain: foam.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/foam-ai/security/foam-ai-domain-security.yml
summary_line: DMARC
tags:
- Company
---
