---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ifood.com.br
  spf: true
hosts:
- cert_expires: Dec 21 04:07:44 2026 GMT
  host: www.ifood.com.br
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ifood Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iFood, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: iFood
provider_slug: ifood
slug: ifood-domain-security
source_filename: ifood-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ifood.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 04:07:44 2026 GMT\n  hsts: null\ndomains:\n- domain: ifood.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ifood/refs/heads/main/security/ifood-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
