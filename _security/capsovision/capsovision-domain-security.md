---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: capsovision.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: capsocloud.com
  spf: false
hosts:
- cert_expires: Sep 13 07:56:36 2026 GMT
  host: capsovision.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: www.capsocloud.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Capsovision Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CapsoVision, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: CapsoVision
provider_slug: capsovision
slug: capsovision-domain-security
source_filename: capsovision-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: capsovision.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 07:56:36 2026 GMT\n  hsts: false\n- host: www.capsocloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: capsovision.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: capsocloud.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capsovision/refs/heads/main/security/capsovision-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Medical Devices
- Healthcare
- Capsule Endoscopy
- Gastroenterology
- Medical Imaging
- Artificial Intelligence
- Cloud Software
---
