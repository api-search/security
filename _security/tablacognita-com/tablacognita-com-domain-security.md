---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: tablacognita.com
  spf: true
hosts:
- host: tablacognita.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: tablacognita-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tablacognita-com, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: tablacognita-com
provider_slug: tablacognita-com
slug: tablacognita-com-domain-security
source_filename: tablacognita-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tablacognita.com\n  https: false\ndomains:\n- domain: tablacognita.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/tablacognita-com/security/tablacognita-com-domain-security.yml
summary_line: DMARC
tags:
- Company
---
