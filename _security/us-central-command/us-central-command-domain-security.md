---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: centcom.mil
  spf: true
hosts:
- cert_expires: Oct  1 05:45:33 2026 GMT
  host: www.centcom.mil
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Us Central Command Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for US Central Command, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: US Central Command
provider_slug: us-central-command
slug: us-central-command-domain-security
source_filename: us-central-command-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.centcom.mil\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 05:45:33 2026 GMT\n  hsts: null\ndomains:\n- domain: centcom.mil\n  dnssec: true\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-central-command/refs/heads/main/security/us-central-command-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Federal Government
- Military
- Department of Defense
- National Security
---
