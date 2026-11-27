---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kamy.dev
  spf: false
hosts:
- cert_expires: Jan 13 11:45:00 2027 GMT
  host: kamy.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: kamy-dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for kamy-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: kamy-dev
provider_slug: kamy-dev
slug: kamy-dev-domain-security
source_filename: kamy-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kamy.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 11:45:00 2027 GMT\n  hsts: null\ndomains:\n- domain: kamy.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/kamy-dev/security/kamy-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
