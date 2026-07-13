---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: public.lu
  spf: false
hosts:
- cert_expires: Mar  6 14:40:00 2027 GMT
  host: data.public.lu
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Government Luxembourg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Government, Luxembourg, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: Open Government, Luxembourg
provider_slug: open-government-luxembourg
slug: open-government-luxembourg-domain-security
source_filename: open-government-luxembourg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.public.lu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 14:40:00 2027 GMT\n  hsts: false\ndomains:\n- domain: public.lu\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-government-luxembourg/refs/heads/main/security/open-government-luxembourg-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Government
- Public APIs
---
