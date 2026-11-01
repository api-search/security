---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: envitia.com
  spf: true
hosts:
- cert_expires: Jan 16 08:30:03 2027 GMT
  host: www.envitia.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Envitia Ltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Envitia Ltd., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Envitia Ltd.
provider_slug: envitia-ltd
slug: envitia-ltd-domain-security
source_filename: envitia-ltd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.envitia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 08:30:03 2027 GMT\n  hsts: false\ndomains:\n- domain: envitia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/envitia-ltd/security/envitia-ltd-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
