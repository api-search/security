---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kubota.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kubotausa.com
  spf: true
hosts:
- cert_expires: Mar 11 14:59:00 2027 GMT
  host: www.kubota.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 17:57:21 2026 GMT
  host: www.kubotausa.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kubota Corporation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kubota Corporation, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kubota Corporation
provider_slug: kubota-corporation
slug: kubota-corporation-domain-security
source_filename: kubota-corporation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kubota.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 14:59:00 2027 GMT\n  hsts: false\n- host: www.kubotausa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 17:57:21 2026 GMT\n  hsts: false\ndomains:\n- domain: kubota.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: kubotausa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kubota-corporation/refs/heads/main/security/kubota-corporation-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Agriculture
- Construction Equipment
- Heavy Equipment
- Manufacturing
- Telematics
---
