---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: expandingweb.com
  spf: true
hosts:
- cert_expires: Jan 17 02:53:41 2027 GMT
  host: expandingweb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Expandingweb Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for expandingweb-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: expandingweb-com
provider_slug: expandingweb-com
slug: expandingweb-com-domain-security
source_filename: expandingweb-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: expandingweb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 02:53:41 2027 GMT\n  hsts: null\ndomains:\n- domain: expandingweb.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/expandingweb-com/security/expandingweb-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
