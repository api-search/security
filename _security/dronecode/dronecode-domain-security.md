---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: px4.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: mavlink.io
  spf: false
- caa: []
  dmarc: true
  dmarc_note: p=none is monitor-only — it publishes a policy without enforcing one. Reports go to the Linux Foundation.
  dmarc_policy: none
  dmarc_record: v=DMARC1; p=none; sp=none; rua=mailto:dmarc+dronecode@linuxfoundation.org
  dnssec: false
  domain: dronecode.org
  source: probed by hand 2026-09-06 (dig CAA/TXT/DNSKEY)
  spf: true
  spf_record: v=spf1 include:forwardemail.net mx include:aspmx.pardot.com include:mailgun.org include:8112310.spf10.hubspotemail.net ~all
hosts:
- cert_expires: Mar 16 23:59:59 2027 GMT
  host: docs.px4.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 04:16:18 2026 GMT
  host: mavsdk.mavlink.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 11:49:19 2026 GMT
  host: mavlink.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 17:59:39 2026 GMT
  host: dronecode.org
  hsts: true
  hsts_max_age: 300
  hsts_note: 'Strict-Transport-Security: max-age=300; includeSubDomains — a 300-second max-age is far below the 31536000 the preload list requires and gives almost no protection.'
  https: true
  source: probed by hand 2026-09-06; probe-domain-security.py collects at most 4 hosts and dropped this one
  tls_version: TLSv1.3
hosts_probed: 4
kind: domain-security
layout: security
method: probed
name: Dronecode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dronecode Foundation, probed live across 4 host(s) and 3 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dronecode Foundation
provider_slug: dronecode
slug: dronecode-domain-security
source_filename: dronecode-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.px4.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 16 23:59:59 2027 GMT\n  hsts: false\n- host: mavsdk.mavlink.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 04:16:18 2026 GMT\n  hsts: false\n- host: mavlink.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 11:49:19 2026 GMT\n  hsts: false\n- host: dronecode.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 17:59:39 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n  hsts_note: 'Strict-Transport-Security: max-age=300; includeSubDomains — a 300-second max-age is far below the\n    31536000 the preload list requires and gives almost no protection.'\n  source: probed by hand 2026-09-06; probe-domain-security.py collects at most 4 hosts and dropped this one\ndomains:\n- domain: px4.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ quarantine\n- domain: mavlink.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: dronecode.org\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:forwardemail.net mx include:aspmx.pardot.com include:mailgun.org include:8112310.spf10.hubspotemail.net\n    ~all\n  dmarc: true\n  dmarc_policy: none\n  dmarc_record: v=DMARC1; p=none; sp=none; rua=mailto:dmarc+dronecode@linuxfoundation.org\n  dmarc_note: p=none is monitor-only — it publishes a policy without enforcing one. Reports go to the Linux Foundation.\n  source: probed by hand 2026-09-06 (dig CAA/TXT/DNSKEY)\nnote: dronecode.org, mavlink.io and px4.io all lack DNSSEC and CAA. mavlink.io publishes neither SPF nor DMARC.\n  Only dronecode.org sets HSTS, and at max-age=300.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dronecode/refs/heads/main/security/dronecode-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Drones
- UAV
- Robotics
- MAVLink
- PX4
- Autopilot
- Aerial Robotics
- gRPC
- Open Source
- Linux Foundation
---
