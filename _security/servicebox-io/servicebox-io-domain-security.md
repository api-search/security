---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: servicebox.io
  spf: true
hosts:
- cert_expires: Jan 18 15:20:45 2027 GMT
  host: servicebox.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Servicebox Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for servicebox-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: servicebox-io
provider_slug: servicebox-io
slug: servicebox-io-domain-security
source_filename: servicebox-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: servicebox.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 15:20:45 2027 GMT\n  hsts: false\ndomains:\n- domain: servicebox.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/servicebox-io/security/servicebox-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Data
- APIs
- Europe
- Turkey
---
