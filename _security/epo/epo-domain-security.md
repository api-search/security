---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:opsec@epo.org"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: epo.org
  spf: true
hosts:
- cert_expires: Dec  6 09:26:35 2026 GMT
  host: developers.epo.org
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Epo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EPO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: EPO
provider_slug: epo
slug: epo-domain-security
source_filename: epo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.epo.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 09:26:35 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: epo.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:opsec@epo.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epo/refs/heads/main/security/epo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Patent
- Public APIs
---
