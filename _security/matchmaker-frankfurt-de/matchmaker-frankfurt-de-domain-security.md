---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: matchmaker-frankfurt.de
  spf: true
hosts:
- cert_expires: Dec 30 17:02:43 2026 GMT
  host: matchmaker-frankfurt.de
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Matchmaker Frankfurt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Matchmaker Frankfurt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Matchmaker Frankfurt
provider_slug: matchmaker-frankfurt-de
slug: matchmaker-frankfurt-de-domain-security
source_filename: matchmaker-frankfurt-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: matchmaker-frankfurt.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 17:02:43 2026 GMT\n  hsts: false\ndomains:\n- domain: matchmaker-frankfurt.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/matchmaker-frankfurt-de/security/matchmaker-frankfurt-de-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Photography
- Dating
- Frankfurt
- Germany
- Services
---
