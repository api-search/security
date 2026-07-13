---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hapag-lloyd.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hlag.com
  spf: true
hosts:
- cert_expires: Aug 17 23:37:17 2026 GMT
  host: www.hapag-lloyd.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: api-portal.hlag.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Hapag Lloyd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hapag-Lloyd, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hapag-Lloyd
provider_slug: hapag-lloyd
slug: hapag-lloyd-domain-security
source_filename: hapag-lloyd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hapag-lloyd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 23:37:17 2026 GMT\n  hsts: null\n- host: api-portal.hlag.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hapag-lloyd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: hlag.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hapag-lloyd/refs/heads/main/security/hapag-lloyd-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Maritime
- Shipping
- Container Logistics
- Supply Chain
---
