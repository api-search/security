---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: meetslava.ru
  spf: true
hosts:
- host: meetslava.ru
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: meetslava-ru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for meetslava-ru, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: meetslava-ru
provider_slug: meetslava-ru
slug: meetslava-ru-domain-security
source_filename: meetslava-ru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meetslava.ru\n  https: false\ndomains:\n- domain: meetslava.ru\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/meetslava-ru/security/meetslava-ru-domain-security.yml
summary_line: DMARC
tags:
- Company
---
