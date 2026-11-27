---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bensaid-avocats.fr
  spf: true
hosts:
- cert_expires: Jan  3 21:44:38 2027 GMT
  host: bensaid-avocats.fr
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bensaid Avocats Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bensaid Avocats, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bensaid Avocats
provider_slug: bensaid-avocats-fr
slug: bensaid-avocats-fr-domain-security
source_filename: bensaid-avocats-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bensaid-avocats.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 21:44:38 2027 GMT\n  hsts: false\ndomains:\n- domain: bensaid-avocats.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bensaid-avocats-fr/security/bensaid-avocats-fr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Law
- Tax
- Wealth
- International
- Real Estate
- Art
---
