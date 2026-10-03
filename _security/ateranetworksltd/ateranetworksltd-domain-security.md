---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: atera.com
  spf: true
hosts:
- cert_expires: Dec 16 13:46:07 2026 GMT
  host: www.atera.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ateranetworksltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ateranetworksltd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Ateranetworksltd
provider_slug: ateranetworksltd
slug: ateranetworksltd-domain-security
source_filename: ateranetworksltd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.atera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 13:46:07 2026 GMT\n  hsts: null\ndomains:\n- domain: atera.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ateranetworksltd/refs/heads/main/security/ateranetworksltd-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- IT Automation
- Remote Access
- MSP
- Software-as-a-Service
- Software
---
