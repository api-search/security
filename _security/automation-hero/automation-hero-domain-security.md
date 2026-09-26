---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: automationhero.com
  spf: true
hosts:
- cert_expires: Mar  9 03:29:44 2027 GMT
  host: automationhero.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Automation Hero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Automation Hero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Automation Hero
provider_slug: automation-hero
slug: automation-hero-domain-security
source_filename: automation-hero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: automationhero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  9 03:29:44 2027 GMT\n  hsts: false\ndomains:\n- domain: automationhero.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/automation-hero/refs/heads/main/security/automation-hero-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
