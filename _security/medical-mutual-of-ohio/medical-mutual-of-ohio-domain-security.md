---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: medmutual.com
  spf: true
hosts:
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: www.medmutual.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Medical Mutual Of Ohio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Medical Mutual of Ohio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Medical Mutual of Ohio
provider_slug: medical-mutual-of-ohio
slug: medical-mutual-of-ohio-domain-security
source_filename: medical-mutual-of-ohio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.medmutual.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: medmutual.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medical-mutual-of-ohio/refs/heads/main/security/medical-mutual-of-ohio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health Insurance
- Healthcare
- Insurance
- Ohio
---
