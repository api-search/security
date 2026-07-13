---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cooperhewitt.org
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: collection.cooperhewitt.org
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Cooper Hewitt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cooper Hewitt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Cooper Hewitt
provider_slug: cooper-hewitt
slug: cooper-hewitt-domain-security
source_filename: cooper-hewitt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: collection.cooperhewitt.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\ndomains:\n- domain: cooperhewitt.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cooper-hewitt/refs/heads/main/security/cooper-hewitt-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Art And Design
- Public APIs
---
