---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: theguardian.com
  spf: true
hosts:
- cert_expires: Sep 21 19:33:19 2026 GMT
  host: open-platform.theguardian.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Guardian Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Guardian, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: The Guardian
provider_slug: the-guardian
slug: the-guardian-domain-security
source_filename: the-guardian-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: open-platform.theguardian.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 19:33:19 2026 GMT\n  hsts: false\ndomains:\n- domain: theguardian.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-guardian/refs/heads/main/security/the-guardian-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- News
- Public APIs
---
