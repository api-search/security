---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: altitudeangel.com
  spf: true
hosts:
- host: www.altitudeangel.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Altitude Angel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Altitude Angel, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Altitude Angel
provider_slug: altitudeangel
slug: altitudeangel-domain-security
source_filename: altitudeangel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.altitudeangel.com\n  https: false\ndomains:\n- domain: altitudeangel.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/altitudeangel/security/altitudeangel-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
---
