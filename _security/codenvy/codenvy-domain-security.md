---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: codenvy.com
  spf: true
hosts:
- host: www.codenvy.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Codenvy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Codenvy, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Codenvy
provider_slug: codenvy
slug: codenvy-domain-security
source_filename: codenvy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.codenvy.com\n  https: false\ndomains:\n- domain: codenvy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/codenvy/security/codenvy-domain-security.yml
summary_line: DMARC
tags:
- Company
---
