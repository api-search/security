---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: councilbox.com
  spf: true
hosts:
- cert_expires: Dec 20 07:54:49 2026 GMT
  host: www.councilbox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Councilbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Councilbox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Councilbox
provider_slug: councilbox
slug: councilbox-domain-security
source_filename: councilbox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.councilbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 07:54:49 2026 GMT\n  hsts: false\ndomains:\n- domain: councilbox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/councilbox/security/councilbox-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- CivicTech
- APIPlatform
- CommunityEngagement
- CloudServices
---
