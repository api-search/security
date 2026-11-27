---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: biohackingkompakt.de
  spf: true
hosts:
- cert_expires: Jan 19 12:08:50 2027 GMT
  host: biohackingkompakt.de
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Biohacking Kompakt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Biohacking Kompakt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Biohacking Kompakt
provider_slug: biohackingkompakt-de
slug: biohackingkompakt-de-domain-security
source_filename: biohackingkompakt-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: biohackingkompakt.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 12:08:50 2027 GMT\n  hsts: false\ndomains:\n- domain: biohackingkompakt.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/biohackingkompakt-de/security/biohackingkompakt-de-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Supplements
- Longevity
- Health
- German
- Fact Checking
---
